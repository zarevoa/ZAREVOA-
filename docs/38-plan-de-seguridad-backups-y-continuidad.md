# ZAREVOA — Plan de Seguridad, Backups y Continuidad

## 1. Objetivo

Este documento define los principios y controles iniciales de seguridad, respaldo y continuidad operacional para ZAREVOA V1.

Su objetivo será proteger:

- Usuarios.
- Cuentas.
- Travel Profiles.
- Viajes.
- Itinerarios.
- Base de datos.
- Código.
- APIs.
- Claves.
- Infraestructura.
- Información empresarial.

La seguridad deberá formar parte de la arquitectura desde el comienzo y no incorporarse únicamente después del lanzamiento.

---

# A. PRINCIPIOS GENERALES

## 2. Seguridad desde el diseño

Cada nueva funcionalidad deberá considerar:

- Qué información utiliza.
- Quién puede acceder.
- Cómo se almacena.
- Cómo se transmite.
- Qué ocurre si falla.
- Qué ocurre si alguien intenta abusar de ella.

---

## 3. Mínimo privilegio

Cada usuario, servicio o componente deberá disponer únicamente de los permisos necesarios para cumplir su función.

No deberán concederse accesos amplios por comodidad.

---

## 4. Defensa por capas

ZAREVOA no deberá depender de una única medida de seguridad.

La protección deberá combinar:

- Autenticación.
- Autorización.
- Cifrado.
- Validación.
- Gestión de secretos.
- Monitoreo.
- Backups.
- Actualizaciones.
- Controles de infraestructura.

---

## 5. Seguridad proporcional

V1 deberá implementar controles sólidos sin construir una infraestructura innecesariamente compleja.

La seguridad deberá evolucionar junto con:

- Cantidad de usuarios.
- Información almacenada.
- Ingresos.
- Integraciones.
- Riesgo.

---

# B. CUENTAS DE USUARIO

## 6. Autenticación

El sistema deberá utilizar mecanismos de autenticación seguros.

Siempre que sea posible, se preferirán soluciones maduras y mantenidas antes que construir un sistema de autenticación propio desde cero.

---

## 7. Contraseñas

Si ZAREVOA gestiona contraseñas directamente:

- Nunca deberán almacenarse en texto plano.
- Deberán utilizarse algoritmos de hash adecuados.
- Deberán aplicarse controles contra ataques automatizados.
- La recuperación deberá realizarse mediante mecanismos seguros.

---

## 8. Sesiones

Las sesiones deberán:

- Ser difíciles de predecir.
- Expirar adecuadamente.
- Poder revocarse.
- Protegerse durante la transmisión.

---

## 9. Recuperación de cuenta

El proceso deberá evitar que una persona pueda apropiarse fácilmente de una cuenta ajena.

Los enlaces o códigos de recuperación deberán:

- Ser temporales.
- Ser de un solo uso cuando corresponda.
- No exponerse públicamente.

---

## 10. Autenticación multifactor

### P1 / P2

Evaluar MFA inicialmente para:

- Administración.
- Accesos internos.
- Funciones especialmente sensibles.

Posteriormente podrá evaluarse para usuarios.

---

# C. AUTORIZACIÓN

## 11. Separación entre usuarios

Un usuario no deberá poder acceder al:

- Travel Profile.
- Viajes.
- Itinerarios.
- Datos.

de otro usuario sin autorización.

---

## 12. Validación del servidor

La autorización no deberá depender únicamente de ocultar botones en la interfaz.

El backend deberá verificar que cada operación está autorizada.

---

## 13. Identificadores

Conocer o adivinar el identificador de un viaje no deberá ser suficiente para acceder a él.

---

# D. ADMINISTRACIÓN

## 14. Cuentas administrativas

Las cuentas con permisos elevados deberán mantenerse al mínimo.

---

## 15. Protección reforzada

Para cuentas administrativas deberán considerarse:

- Contraseñas únicas.
- MFA.
- Registro de accesos.
- Revocación inmediata cuando corresponda.

---

## 16. Uso separado

Siempre que sea posible, las funciones administrativas deberán mantenerse separadas del uso cotidiano.

---

# E. BASE DE DATOS

## 17. Acceso

La base de datos no deberá exponerse públicamente de forma innecesaria.

---

## 18. Credenciales

Las credenciales deberán almacenarse mediante mecanismos seguros de secretos.

Nunca deberán incorporarse directamente al código fuente.

---

## 19. Permisos

Los servicios deberán disponer únicamente de los permisos necesarios.

---

## 20. Datos

La estructura deberá evitar exposición innecesaria de información personal.

---

## 21. Cifrado

Cuando el proveedor lo permita, utilizar:

- Cifrado en tránsito.
- Cifrado en reposo.

---

# F. TRANSMISIÓN

## 22. HTTPS

Todo tráfico público de ZAREVOA deberá utilizar HTTPS.

---

## 23. Información sensible

No deberá transmitirse información sensible mediante canales inseguros.

---

## 24. Certificados

Los certificados deberán:

- Mantenerse vigentes.
- Renovarse automáticamente cuando sea posible.
- Monitorearse.

---

# G. GESTIÓN DE SECRETOS

## 25. Qué se considera secreto

Entre otros:

- Claves de IA.
- Claves de APIs.
- Credenciales de base de datos.
- Tokens.
- Claves de pago.
- Credenciales administrativas.
- Secretos de autenticación.

---

## 26. Repositorio

**Ningún secreto deberá almacenarse en GitHub dentro del código o documentación pública.**

---

## 27. Variables de entorno

Los secretos deberán gestionarse mediante:

- Variables de entorno.
- Gestores de secretos.
- Sistemas equivalentes del proveedor.

---

## 28. Rotación

Una clave deberá rotarse inmediatamente si:

- Se expone.
- Se publica accidentalmente.
- Existe sospecha de compromiso.
- Un proveedor lo recomienda por seguridad.

---

## 29. Claves separadas

Cuando sea posible deberán utilizarse credenciales distintas para:

- Desarrollo.
- Pruebas.
- Producción.

---

# H. GITHUB Y CÓDIGO

## 30. Protección del repositorio

La cuenta y repositorio de GitHub deberán protegerse mediante:

- Contraseña única.
- MFA.
- Control de accesos.
- Revisión periódica de colaboradores.

---

## 31. Rama principal

Cuando el desarrollo aumente deberá evaluarse protección de la rama principal.

Podrá incluir:

- Pull requests.
- Revisiones.
- Checks automáticos.
- Restricciones de escritura directa.

---

## 32. Historial

Eliminar una clave del archivo actual no significa necesariamente eliminarla del historial de Git.

Si un secreto se publica:

**deberá considerarse comprometido y rotarse.**

---

## 33. Dependencias

Las dependencias deberán:

- Mantenerse actualizadas.
- Revisarse ante vulnerabilidades.
- Evitar paquetes innecesarios.
- Proceder de fuentes confiables.

---

# I. DESARROLLO SEGURO

## 34. Validación de entradas

Todo dato recibido deberá considerarse potencialmente no confiable.

Validar:

- Tipo.
- Formato.
- Longitud.
- Valores permitidos.
- Tamaño.

---

## 35. Frontend y backend

La validación del frontend mejora la experiencia.

La validación del backend protege el sistema.

Por ello, las operaciones importantes deberán validarse en el servidor.

---

## 36. Consultas

Deberán utilizarse mecanismos seguros de acceso a datos para reducir riesgos como inyección.

---

## 37. Contenido generado

Cuando se muestre contenido generado por usuarios o sistemas externos deberá tratarse de forma segura para evitar ejecución no deseada de código o contenido malicioso.

---

# J. APIs

## 38. Claves privadas

Las claves privadas de APIs no deberán enviarse al navegador cuando no sea necesario.

---

## 39. Backend

Las integraciones sensibles deberán ejecutarse desde el backend.

---

## 40. Límites

Deberán utilizarse:

- Rate limits.
- Cuotas.
- Alertas.
- Límites de gasto.

cuando los proveedores lo permitan.

---

## 41. Fallos

Una API externa puede:

- Caerse.
- Responder lentamente.
- Cambiar.
- Entregar información incompleta.

ZAREVOA deberá manejar estos casos sin comprometer la estabilidad general.

---

# K. INTELIGENCIA ARTIFICIAL

## 42. Protección de claves

Las claves del proveedor de IA deberán mantenerse exclusivamente en entornos seguros.

---

## 43. Datos enviados

Enviar únicamente la información necesaria para la tarea.

---

## 44. Prompt injection y contenido externo

Si ZAREVOA procesa contenido externo, deberá asumir que dicho contenido puede contener instrucciones maliciosas o manipuladoras.

El sistema deberá separar:

- Datos.
- Instrucciones internas.
- Acciones autorizadas.

---

## 45. Acciones de IA

La IA no deberá disponer automáticamente de permisos ilimitados para:

- Modificar datos.
- Realizar pagos.
- Borrar información.
- Ejecutar acciones sensibles.

Las acciones deberán estar controladas por reglas y permisos.

---

## 46. Validación del resultado

Los resultados relevantes del ZAREVOA Engine deberán pasar por controles estructurados antes de mostrarse cuando corresponda.

---

# L. PROTECCIÓN CONTRA ABUSO

## 47. Rate limiting

Deberán existir límites razonables para prevenir:

- Bots.
- Spam.
- Generaciones masivas.
- Ataques automatizados.
- Consumo excesivo de APIs.

---

## 48. Costos

La protección contra abuso también será una medida financiera.

Un atacante no deberá poder generar fácilmente costos ilimitados mediante llamadas repetidas a IA o APIs.

---

## 49. Límites por usuario

Podrán establecerse límites según:

- Cuenta.
- IP.
- Función.
- Período.
- Tipo de plan.

---

# M. LOGS

## 50. Objetivo

Los logs deberán ayudar a:

- Detectar errores.
- Investigar incidentes.
- Analizar rendimiento.
- Proteger el sistema.

---

## 51. Datos en logs

No deberán registrarse innecesariamente:

- Contraseñas.
- Tokens.
- Claves.
- Información de pago completa.
- Datos personales innecesarios.

---

## 52. Acceso

Los logs deberán estar disponibles únicamente para personas o sistemas autorizados.

---

## 53. Retención

La retención deberá ser suficiente para operación y seguridad, pero no indefinida sin necesidad.

---

# N. MONITOREO

## 54. Componentes

Monitorear:

- Aplicación.
- Base de datos.
- APIs.
- IA.
- Autenticación.
- Rendimiento.
- Errores.
- Costos.

---

## 55. Alertas

Configurar progresivamente alertas para:

- Caídas.
- Aumento anormal de errores.
- Fallos de base de datos.
- Costos anormales.
- Uso excesivo de APIs.
- Problemas de almacenamiento.

---

## 56. Alertas útiles

Evitar crear tantas alertas que terminen siendo ignoradas.

Cada alerta importante deberá indicar una situación que pueda requerir acción.

---

# O. BACKUPS

## 57. Principio

Un backup no existe realmente hasta que puede restaurarse.

---

## 58. Qué respaldar

Como mínimo evaluar respaldo de:

- Base de datos.
- Configuraciones críticas.
- Información necesaria para recuperación.
- Código y documentación.

El código almacenado correctamente en GitHub ya dispone de historial, pero no reemplaza los backups de otros sistemas.

---

## 59. Automatización

Los backups de producción deberán automatizarse siempre que sea posible.

---

## 60. Frecuencia

La frecuencia dependerá de:

- Cantidad de cambios.
- Volumen de usuarios.
- Criticidad.
- Capacidades del proveedor.

Para V1 podrá utilizarse inicialmente el sistema automatizado de backups del proveedor, siempre que cumpla los requisitos definidos.

---

## 61. Retención de backups

Deberán existir varias versiones cuando sea viable.

No depender exclusivamente del último backup.

---

## 62. Separación

Siempre que sea posible, los backups críticos no deberán depender completamente del mismo punto de fallo que los datos originales.

---

# P. RESTAURACIÓN

## 63. Prueba

Deberán realizarse pruebas periódicas de restauración.

---

## 64. Pregunta fundamental

El equipo deberá poder responder:

**Si la base de datos desapareciera hoy, ¿cómo restauraríamos ZAREVOA?**

---

## 65. Procedimiento

Documentar:

1. Identificar el incidente.
2. Detener operaciones peligrosas si corresponde.
3. Seleccionar backup.
4. Restaurar.
5. Validar integridad.
6. Reactivar servicio.
7. Investigar causa.

---

# Q. RPO Y RTO

## 66. Recovery Point Objective

RPO representa cuánta información podría perderse como máximo entre el último respaldo válido y el incidente.

---

## 67. Recovery Time Objective

RTO representa cuánto tiempo se espera necesitar para recuperar el servicio.

---

## 68. V1

Los valores definitivos deberán establecerse según:

- Arquitectura.
- Costos.
- Número de usuarios.
- Importancia del servicio.

No será necesario diseñar inicialmente niveles de disponibilidad propios de infraestructura crítica, pero sí deberá existir una expectativa razonable de recuperación.

---

# R. CONTINUIDAD OPERACIONAL

## 69. Objetivo

ZAREVOA deberá poder continuar o recuperarse ante fallos razonablemente previsibles.

---

## 70. Escenarios

Preparar respuesta para:

- Caída del hosting.
- Caída de base de datos.
- Fallo del proveedor de IA.
- Fallo de una API.
- Error de despliegue.
- Eliminación accidental.
- Cuenta comprometida.
- Clave expuesta.
- Aumento inesperado de tráfico.

---

# S. FALLO DE IA

## 71. Proveedor no disponible

Si la IA no responde, ZAREVOA deberá:

- Detectar el problema.
- Evitar resultados incompletos presentados como válidos.
- Informar al usuario de forma comprensible.
- Permitir reintentar cuando corresponda.

---

## 72. Estrategia futura

Podrá evaluarse soporte para proveedores alternativos si la escala y dependencia lo justifican.

No será obligatorio para V1 si añade complejidad excesiva.

---

# T. FALLO DE APIs EXTERNAS

## 73. Degradación

Una API secundaria no deberá necesariamente inutilizar toda la plataforma.

Cuando sea posible, utilizar degradación controlada.

---

## 74. Datos no disponibles

Si no puede verificarse un dato:

**no deberá inventarse.**

La interfaz podrá indicar que esa información no está disponible temporalmente.

---

# U. DESPLIEGUES

## 75. Proceso

Los despliegues deberán ser repetibles y controlados.

---

## 76. Entornos

Mantener cuando sea viable:

- Desarrollo.
- Pruebas/staging.
- Producción.

---

## 77. Pruebas antes de producción

Antes de desplegar cambios relevantes:

- Ejecutar pruebas.
- Revisar errores.
- Validar variables.
- Verificar migraciones.

---

## 78. Rollback

Deberá existir una forma razonable de volver a una versión anterior cuando un despliegue produzca problemas graves.

---

# V. MIGRACIONES DE BASE DE DATOS

## 79. Control

Las migraciones deberán:

- Versionarse.
- Probarse.
- Ejecutarse de forma controlada.

---

## 80. Cambios destructivos

Antes de eliminar o transformar datos importantes deberá existir:

- Backup.
- Plan de reversión cuando sea posible.
- Validación.

---

# W. INCIDENTES

## 81. Definición

Un incidente puede incluir:

- Acceso no autorizado.
- Exposición de datos.
- Caída.
- Pérdida de información.
- Clave comprometida.
- Ataque.
- Error grave de configuración.

---

## 82. Proceso

Ante un incidente:

**Detectar**

↓

**Clasificar**

↓

**Contener**

↓

**Investigar**

↓

**Corregir**

↓

**Restaurar**

↓

**Documentar**

↓

**Prevenir recurrencia**

---

# X. SEVERIDAD DE INCIDENTES

## 83. Crítico

Ejemplos:

- Exposición significativa de datos.
- Compromiso administrativo.
- Pérdida grave de datos.
- Servicio completamente inutilizable.

Respuesta:

**Prioridad inmediata.**

---

## 84. Alto

Impacto significativo sobre usuarios o funciones esenciales.

---

## 85. Medio

Problema limitado con alternativa disponible.

---

## 86. Bajo

Impacto menor.

---

# Y. PLAN DE RESPUESTA

## 87. Registro inicial

Registrar:

- Fecha.
- Hora.
- Sistema.
- Síntoma.
- Impacto.
- Personas o servicios afectados.

---

## 88. Contención

La prioridad inicial podrá ser:

- Revocar una clave.
- Bloquear una cuenta.
- Desactivar una función.
- Detener un despliegue.
- Aislar un componente.

---

## 89. Evidencia

Evitar eliminar información necesaria para investigar el incidente.

---

## 90. Recuperación

Antes de declarar resuelto:

- Confirmar funcionamiento.
- Verificar seguridad.
- Revisar integridad.
- Monitorear recurrencia.

---

# Z. POSTMORTEM

## 91. Incidentes relevantes

Después de un incidente importante deberá documentarse:

- Qué ocurrió.
- Impacto.
- Causa.
- Cómo se detectó.
- Cómo se resolvió.
- Qué se cambiará.

---

## 92. Objetivo

El postmortem deberá centrarse en mejorar sistemas y procesos.

---

# AA. COMUNICACIÓN

## 93. Usuarios afectados

Cuando corresponda legal u operacionalmente, deberá comunicarse el incidente de forma:

- Clara.
- Precisa.
- Oportuna.
- Sin ocultar información relevante.
- Sin especular sobre hechos no confirmados.

---

## 94. Notificaciones legales

Los incidentes relacionados con datos personales deberán evaluarse según las obligaciones de notificación aplicables.

---

# AB. PROVEEDORES

## 95. Dependencias críticas

Mantener inventario de:

- Hosting.
- Base de datos.
- IA.
- Autenticación.
- APIs.
- Correo.
- Pagos.
- Analítica.

---

## 96. Accesos

Cuando un proveedor deje de utilizarse:

- Revocar claves.
- Eliminar accesos.
- Revisar datos almacenados.
- Actualizar documentación.

---

# AC. PAGOS

## 97. Proveedor especializado

Cuando se activen pagos, utilizar proveedores especializados.

---

## 98. PCI y tarjetas

ZAREVOA deberá minimizar al máximo su exposición directa a información de tarjetas y seguir los requisitos aplicables del proveedor y estándares correspondientes.

---

## 99. Webhooks

Las notificaciones de pago deberán:

- Verificarse.
- Autenticarse según mecanismo del proveedor.
- Procesarse de forma segura.

---

# AD. PRIVACIDAD Y SEGURIDAD

## 100. Relación

Privacidad y seguridad son conceptos diferentes pero relacionados.

Privacidad define:

**qué datos deben utilizarse y por qué.**

Seguridad ayuda a proteger:

**esos datos frente a acceso, pérdida o modificación no autorizada.**

---

# AE. DATOS DE PRODUCCIÓN

## 101. Desarrollo

Siempre que sea posible, evitar utilizar datos personales reales de producción para pruebas de desarrollo.

---

## 102. Datos de prueba

Preferir:

- Datos ficticios.
- Datos anonimizados.
- Conjuntos específicamente creados para pruebas.

---

# AF. ELIMINACIÓN

## 103. Eliminación de cuenta

Cuando se implemente eliminación de cuenta, deberá definirse qué información:

- Se elimina inmediatamente.
- Se elimina posteriormente.
- Debe conservarse legalmente.
- Puede permanecer temporalmente en backups.

---

## 104. Backups

La política de privacidad deberá reflejar adecuadamente cómo funciona la eliminación respecto de copias de seguridad cuando corresponda.

---

# AG. DISPOSITIVOS Y ACCESOS INTERNOS

## 105. Equipos

Los dispositivos utilizados para administrar ZAREVOA deberán protegerse mediante:

- Bloqueo.
- Actualizaciones.
- Contraseñas.
- Cifrado cuando esté disponible.
- Software confiable.

---

## 106. Redes

Evitar operaciones administrativas sensibles desde redes no confiables sin medidas adecuadas de protección.

---

# AH. PHISHING E INGENIERÍA SOCIAL

## 107. Riesgo

No todos los ataques serán técnicos.

Podrán intentar obtener:

- Contraseñas.
- Claves.
- Accesos.
- Información empresarial.

mediante engaño.

---

## 108. Verificación

Las solicitudes sensibles deberán verificarse antes de entregar información o cambiar accesos.

---

# AI. DOMINIO

## 109. Protección

La cuenta del registrador del dominio deberá disponer de:

- Contraseña única.
- MFA.
- Datos de recuperación actualizados.

---

## 110. DNS

Los cambios DNS deberán limitarse a usuarios autorizados.

Un compromiso del dominio podría afectar toda la confianza de ZAREVOA.

---

# AJ. CORREO

## 111. Cuenta principal

Las cuentas de correo administrativas deberán protegerse especialmente.

---

## 112. Autenticación del dominio

Cuando se configure correo empresarial deberán implementarse progresivamente mecanismos apropiados de autenticación del correo para reducir suplantación y mejorar entregabilidad.

---

# AK. COSTOS Y SEGURIDAD

## 113. Alertas financieras

Configurar alertas de gasto en:

- Hosting.
- IA.
- APIs.
- Servicios cloud.

---

## 114. Límites

Cuando el proveedor lo permita, establecer límites razonables para evitar facturas inesperadas por:

- Error.
- Bucle.
- Ataque.
- Abuso.

---

# AL. PRUEBAS DE SEGURIDAD

## 115. Antes del lanzamiento

Revisar al menos:

- Autenticación.
- Autorización.
- Acceso entre usuarios.
- Validación.
- Gestión de secretos.
- APIs.
- Configuración.
- Dependencias.
- Backups.

---

## 116. Pruebas automatizadas

Incorporar progresivamente:

- Análisis de dependencias.
- Detección de secretos.
- Pruebas de código.
- Checks de despliegue.

---

## 117. Revisión externa

Cuando ZAREVOA alcance mayor escala o maneje información/operaciones de mayor riesgo, deberá evaluarse una revisión de seguridad externa.

---

# AM. CHECKLIST PRE-LANZAMIENTO

## 118. Cuentas

- [ ] Autenticación segura.
- [ ] Recuperación probada.
- [ ] Sesiones seguras.
- [ ] Autorización validada.
- [ ] MFA administrativo.

---

## 119. Infraestructura

- [ ] HTTPS.
- [ ] Producción separada.
- [ ] Base de datos protegida.
- [ ] Backups activos.
- [ ] Restauración probada.
- [ ] Monitoreo activo.

---

## 120. Secretos

- [ ] No existen claves en GitHub.
- [ ] Variables protegidas.
- [ ] Claves separadas por entorno cuando corresponda.
- [ ] Procedimiento de rotación conocido.

---

## 121. Aplicación

- [ ] Entradas validadas.
- [ ] Permisos revisados.
- [ ] Rate limits.
- [ ] Manejo de errores.
- [ ] Logs seguros.

---

## 122. APIs e IA

- [ ] Claves privadas protegidas.
- [ ] Límites de gasto.
- [ ] Fallos controlados.
- [ ] Datos enviados minimizados.
- [ ] Resultados críticos validados.

---

## 123. Código

- [ ] Dependencias revisadas.
- [ ] Rama principal protegida cuando corresponda.
- [ ] Historial sin secretos válidos expuestos.
- [ ] Proceso de despliegue definido.

---

## 124. Incidentes

- [ ] Procedimiento documentado.
- [ ] Accesos para actuar disponibles.
- [ ] Contactos de proveedores identificados.
- [ ] Método de comunicación preparado.

---

# AN. CHECKLIST DE BACKUPS

## 125. Verificación

- [ ] Backup automático activo.
- [ ] Frecuencia conocida.
- [ ] Retención conocida.
- [ ] Ubicación conocida.
- [ ] Acceso protegido.
- [ ] Restauración probada.
- [ ] Resultado documentado.

---

# AO. REVISIÓN PERIÓDICA

## 126. Semanal durante lanzamiento

Revisar:

- Errores.
- Alertas.
- Costos.
- Dependencias críticas.
- Fallos de proveedores.

---

## 127. Mensual

Revisar:

- Accesos.
- Backups.
- Restauración.
- Dependencias.
- Cuentas administrativas.
- Claves relevantes.

---

## 128. Después de cambios importantes

Realizar revisión adicional después de:

- Nueva integración.
- Nuevo proveedor.
- Pagos.
- Journey.
- Cambios de autenticación.
- Cambios importantes de infraestructura.

---

# AP. ESCALABILIDAD DE SEGURIDAD

## 129. V1

Prioridades:

- Cuentas.
- Datos.
- Secretos.
- HTTPS.
- Backups.
- Monitoreo.
- Rate limiting.
- Dependencias.
- Incidentes.

---

## 130. Crecimiento

Añadir progresivamente:

- Controles más avanzados.
- Mayor observabilidad.
- Automatización.
- Revisiones externas.
- Gestión avanzada de accesos.

---

## 131. Journey

Si Journey utiliza:

- Ubicación.
- Notificaciones.
- Información durante el viaje.

deberán revisarse los riesgos específicos antes de activarlos.

---

## 132. Personal

Si Personal incorpora acceso humano a viajes de usuarios, deberán definirse:

- Permisos.
- Registro de acceso.
- Confidencialidad.
- Minimización.

---

# AQ. CONTINUIDAD EMPRESARIAL

## 133. Accesos críticos

ZAREVOA deberá mantener un inventario seguro de los servicios esenciales.

Por ejemplo:

- Dominio.
- GitHub.
- Hosting.
- Base de datos.
- Correo.
- IA.
- APIs.
- Pagos.

---

## 134. Recuperación

Deberá existir una forma documentada de recuperar acceso a servicios críticos sin depender exclusivamente de una única contraseña, dispositivo o punto de fallo.

---

## 135. Documentación

Los procedimientos críticos deberán documentarse suficientemente para evitar depender únicamente de la memoria de una persona.

---

# AR. QUÉ NO HACER

## 136. Prácticas prohibidas

ZAREVOA no deberá:

- Guardar contraseñas en texto plano.
- Publicar claves.
- Compartir credenciales innecesariamente.
- Dar permisos administrativos por comodidad.
- Desactivar controles de seguridad para acelerar un lanzamiento.
- Ignorar alertas de vulnerabilidades críticas.
- Confiar en backups nunca probados.
- Utilizar datos reales innecesariamente en desarrollo.
- Presentar información inventada cuando falla una API.
- Ocultar incidentes relevantes que deban comunicarse.

---

# AS. REGISTRO DE RIESGOS

## 137. Riesgos técnicos

Mantener progresivamente un registro de riesgos con:

- Riesgo.
- Probabilidad.
- Impacto.
- Mitigación.
- Responsable.
- Estado.

---

## 138. Riesgos iniciales

Entre los riesgos a controlar:

- Compromiso de cuenta.
- Exposición de claves.
- Pérdida de datos.
- Costos inesperados.
- Fallo de proveedor.
- Vulnerabilidad de dependencia.
- Acceso indebido entre usuarios.
- Error de despliegue.
- Abuso de IA.

---

# AT. MÉTRICAS DE SEGURIDAD

## 139. Medición

Podrán registrarse:

- Incidentes.
- Tiempo de detección.
- Tiempo de recuperación.
- Restauraciones.
- Fallos de login.
- Uso anormal.
- Vulnerabilidades críticas abiertas.

---

## 140. Objetivo

La finalidad de estas métricas será mejorar la capacidad de prevención y respuesta.

No simplemente producir estadísticas.

---

# AU. RESPONSABILIDAD

## 141. Propietario

Cada sistema crítico deberá tener claramente definido quién o qué proceso es responsable de:

- Mantenerlo.
- Revisarlo.
- Actualizarlo.
- Responder cuando falla.

---

# AV. PRINCIPIO DE RECUPERACIÓN

## 142. Asumir que algo fallará

Ningún sistema es infalible.

Por ello, además de intentar prevenir fallos, ZAREVOA deberá estar preparado para recuperarse.

---

## 143. Preguntas esenciales

Antes del lanzamiento deberán poder responderse estas preguntas:

1. ¿Qué hacemos si GitHub se compromete?
2. ¿Qué hacemos si una clave de IA se publica?
3. ¿Qué hacemos si la base de datos falla?
4. ¿Qué hacemos si eliminamos datos accidentalmente?
5. ¿Qué hacemos si un proveedor deja de responder?
6. ¿Qué hacemos si un despliegue rompe producción?
7. ¿Qué hacemos si los costos aumentan de forma anormal?
8. ¿Cómo recuperamos ZAREVOA desde un backup?

Si una respuesta depende únicamente de improvisar en el momento, el procedimiento deberá mejorarse.

---

# AW. PRINCIPIO FINAL

## 144. Seguridad como parte de la confianza

ZAREVOA manejará información que representa algo importante para el usuario:

**sus viajes.**

Un itinerario puede contener semanas o meses de planificación.

Perderlo, exponerlo o permitir que otra persona lo modifique puede destruir rápidamente la confianza construida por el producto.

Por ello, seguridad, backups y continuidad deberán considerarse parte de la experiencia del usuario, aunque normalmente sean invisibles.

---

## 145. Regla final

ZAREVOA deberá trabajar bajo cuatro principios:

**Prevenir cuando sea posible.**

**Detectar cuando algo falle.**

**Responder de forma controlada.**

**Recuperarse con la menor pérdida posible.**

La seguridad absoluta no existe.

Lo que sí puede construirse es una plataforma preparada, responsable y capaz de aprender de sus incidentes.

Ese deberá ser el estándar de ZAREVOA desde V1.

---

**Estado del documento:** Plan oficial inicial de seguridad, backups, recuperación y continuidad operacional de ZAREVOA V1.
