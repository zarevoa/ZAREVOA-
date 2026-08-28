# 55 — Plan de seguridad, privacidad y protección de datos de ZAREVOA

## 1. Objetivo

Este documento define los principios de seguridad, privacidad y protección de datos que deberán aplicarse en ZAREVOA desde su primera versión.

ZAREVOA podrá manejar información relacionada con:

- cuentas de usuario;
- preferencias de viaje;
- destinos;
- fechas;
- presupuestos;
- composición del grupo;
- itinerarios;
- pagos;
- interacciones con la plataforma.

La protección de esta información deberá formar parte del diseño del producto desde el comienzo.

El principio central será:

> ZAREVOA deberá recopilar únicamente los datos necesarios, protegerlos adecuadamente y utilizarlos únicamente para finalidades legítimas y comprensibles para el usuario.

---

## 2. Seguridad desde el diseño

La seguridad no deberá incorporarse únicamente después del lanzamiento.

Cada nueva funcionalidad deberá considerar:

- qué información utiliza;
- dónde se almacena;
- quién puede acceder;
- durante cuánto tiempo se conserva;
- qué ocurriría si fuera expuesta;
- qué controles necesita.

La seguridad deberá formar parte del proceso de desarrollo.

---

## 3. Privacidad desde el diseño

ZAREVOA deberá aplicar el principio de:

**Privacy by Design.**

Esto significa que la privacidad deberá incorporarse desde la concepción de cada función.

También deberá aplicarse:

**Privacy by Default.**

Las configuraciones iniciales deberán proteger razonablemente al usuario sin exigir conocimientos técnicos.

---

## 4. Minimización de datos

ZAREVOA no deberá recopilar información simplemente porque pueda resultar útil en algún momento.

Cada dato deberá responder:

> ¿Por qué necesitamos esta información?

Si no existe una finalidad suficientemente clara, deberá evitarse su recopilación.

---

## 5. Travel Profile

El Travel Profile será uno de los principales conjuntos de información de ZAREVOA.

Podrá incluir:

- origen;
- destino;
- fechas;
- duración;
- número de viajeros;
- edades cuando sean relevantes;
- presupuesto;
- intereses;
- ritmo;
- preferencias;
- Must See;
- restricciones.

Estos datos deberán utilizarse principalmente para mejorar la planificación.

---

## 6. Datos necesarios versus opcionales

Los campos deberán clasificarse cuando corresponda en:

### Necesarios

Información indispensable para entregar la función.

### Opcionales

Información que puede mejorar la personalización pero que no es estrictamente necesaria.

El usuario deberá poder comprender esta diferencia.

---

## 7. Información sensible

ZAREVOA deberá evitar solicitar información sensible que no sea necesaria para planificar un viaje.

Cuando determinadas necesidades personales afecten el viaje, deberá evaluarse cuidadosamente qué información realmente necesita conocer la plataforma.

Siempre que sea posible deberá utilizarse una preferencia funcional en lugar de información médica o personal detallada.

---

## 8. Ejemplo de minimización

En lugar de solicitar:

**“Indica tu condición médica.”**

podría ser suficiente preguntar:

**“¿Necesitas reducir caminatas o esfuerzo físico?”**

El Engine necesita comprender la necesidad de planificación.

No necesariamente necesita conocer su causa.

---

## 9. Datos de menores

Cuando un viaje incluya menores de edad deberá evitarse recopilar información innecesaria sobre ellos.

Cuando la edad sea útil para planificación podrá utilizarse únicamente con esa finalidad.

La plataforma deberá evaluar las obligaciones legales adicionales aplicables cuando corresponda.

---

## 10. Cuenta de usuario

Los datos básicos de cuenta deberán limitarse inicialmente a lo necesario.

Podrán incluir:

- correo electrónico;
- nombre o identificador;
- preferencias básicas;
- configuración;
- historial necesario.

No deberán solicitarse datos adicionales sin una razón clara.

---

## 11. Contraseñas

Las contraseñas nunca deberán almacenarse en texto plano.

Deberán utilizarse mecanismos modernos y seguros de autenticación y almacenamiento.

Cuando sea posible podrá utilizarse un proveedor especializado de identidad.

Esto permitirá reducir la superficie de riesgo.

---

## 12. Autenticación

La autenticación deberá proteger el acceso a:

- cuenta;
- viajes;
- preferencias;
- productos adquiridos;
- información privada.

Los mecanismos deberán equilibrar:

**Seguridad + facilidad de uso.**

---

## 13. Autenticación multifactor

En etapas posteriores podrá ofrecerse autenticación multifactor.

Deberá priorizarse especialmente para:

- cuentas administrativas;
- colaboradores;
- sistemas internos;
- accesos sensibles.

Las cuentas con privilegios elevados deberán recibir mayor protección.

---

## 14. Sesiones

Las sesiones deberán administrarse de forma segura.

Deberán considerarse:

- expiración;
- revocación;
- cierre de sesión;
- dispositivos;
- cookies seguras;
- tokens.

Una sesión comprometida no deberá permanecer activa indefinidamente.

---

## 15. Autorización

Autenticar a un usuario no significa que pueda acceder a todos los recursos.

Cada solicitud deberá comprobar:

> ¿Este usuario tiene autorización para acceder a este recurso?

Un usuario nunca deberá poder visualizar o modificar viajes pertenecientes a otra cuenta.

---

## 16. Principio de mínimo privilegio

Cada usuario, servicio o colaborador deberá recibir únicamente los permisos necesarios para cumplir su función.

Este principio deberá aplicarse a:

- administradores;
- soporte;
- desarrolladores;
- sistemas;
- APIs;
- bases de datos.

Menos privilegios significan menor impacto potencial ante un incidente.

---

## 17. Roles internos

A medida que crezca el equipo deberán definirse roles.

Ejemplos:

- administración;
- soporte;
- desarrollo;
- operaciones;
- finanzas;
- seguridad.

Cada rol deberá tener permisos específicos.

---

## 18. Acceso de soporte

El equipo de soporte no deberá tener acceso ilimitado a toda la información de todos los usuarios.

Cuando necesite investigar un caso deberá acceder únicamente a lo necesario.

Los accesos sensibles deberán poder registrarse.

---

## 19. Datos en tránsito

La comunicación entre:

- usuario;
- aplicación;
- servidores;
- APIs;
- proveedores;

deberá utilizar conexiones cifradas.

El tráfico sensible no deberá transmitirse mediante canales inseguros.

---

## 20. Datos almacenados

Los datos sensibles deberán protegerse adecuadamente durante su almacenamiento.

Cuando corresponda deberá utilizarse cifrado proporcionado por infraestructura o servicios especializados.

También deberán protegerse:

- backups;
- archivos;
- registros;
- secretos.

---

## 21. Secretos

Las credenciales técnicas nunca deberán almacenarse directamente dentro del código público.

Esto incluye:

- API keys;
- contraseñas;
- tokens;
- secretos de servicios;
- credenciales de bases de datos.

Deberán utilizarse mecanismos seguros de gestión de secretos y variables de entorno.

---

## 22. GitHub y repositorios

Los repositorios deberán mantenerse libres de información confidencial.

Antes de publicar cambios deberá evitarse incluir accidentalmente:

- claves;
- tokens;
- contraseñas;
- datos reales de usuarios;
- archivos de configuración sensibles.

Un secreto eliminado posteriormente del archivo puede continuar existiendo en el historial del repositorio.

---

## 23. Separación de entornos

Deberán distinguirse progresivamente:

- desarrollo;
- pruebas;
- producción.

Los datos reales de usuarios no deberán copiarse innecesariamente a entornos de desarrollo.

Cuando se necesiten datos de prueba deberán preferirse datos ficticios o anonimizados.

---

## 24. Producción

El entorno de producción deberá tener controles más estrictos.

El acceso deberá limitarse a quienes realmente lo necesiten.

Las acciones críticas deberán ser rastreables cuando corresponda.

---

## 25. Base de datos

La base de datos deberá protegerse mediante:

- autenticación;
- permisos;
- redes adecuadas;
- cifrado;
- backups;
- monitoreo.

No deberá exponerse directamente a Internet salvo que exista una razón técnica y controles adecuados.

---

## 26. Backups

ZAREVOA deberá contar progresivamente con copias de seguridad de la información necesaria.

Los backups deberán ser:

- periódicos;
- protegidos;
- verificables;
- recuperables.

Tener una copia que nunca se ha probado no garantiza recuperación.

---

## 27. Pruebas de recuperación

Periódicamente deberá comprobarse que los backups puedan restaurarse.

El proceso deberá responder:

- qué se recupera;
- cuánto tarda;
- cuánto dato podría perderse;
- quién ejecuta la recuperación.

Esto deberá coordinarse con el plan de continuidad de ZAREVOA.

---

## 28. Disponibilidad

La seguridad también incluye mantener el servicio disponible.

Deberán existir medidas frente a:

- fallos;
- abuso;
- tráfico anormal;
- errores;
- proveedores caídos;
- pérdida de datos.

La resiliencia deberá aumentar con el crecimiento.

---

## 29. APIs

Las APIs deberán protegerse mediante:

- autenticación;
- autorización;
- validación;
- límites;
- monitoreo;
- control de errores.

Nunca deberá confiarse automáticamente en información recibida desde el cliente.

---

## 30. Validación de entradas

Toda información enviada por usuarios deberá considerarse potencialmente no confiable.

Deberán aplicarse controles frente a:

- entradas inválidas;
- inyecciones;
- contenido malicioso;
- tamaños excesivos;
- formatos inesperados.

La validación deberá producirse en los lugares apropiados del sistema.

---

## 31. Rate Limiting

Cuando corresponda deberán existir límites de uso para proteger:

- autenticación;
- APIs;
- generación con IA;
- formularios;
- servicios costosos.

Esto ayudará a reducir:

- abuso;
- automatización no autorizada;
- ataques;
- costos inesperados.

---

## 32. Dependencias

Las librerías y componentes externos pueden introducir vulnerabilidades.

Deberán mantenerse procesos para:

- identificar dependencias;
- revisar actualizaciones;
- detectar vulnerabilidades;
- actualizar componentes críticos.

No deberá ignorarse una vulnerabilidad conocida únicamente porque el sistema continúa funcionando.

---

## 33. Proveedores externos

Cada proveedor que procese información deberá evaluarse según:

- seguridad;
- privacidad;
- reputación;
- ubicación de datos;
- términos;
- cumplimiento;
- necesidad real.

La responsabilidad de ZAREVOA no desaparece simplemente porque un tercero procese los datos.

---

## 34. IA y privacidad

La información enviada a proveedores de IA deberá limitarse a lo necesario.

Deberá evitarse enviar datos identificables cuando no sean necesarios para la tarea.

Siempre que sea posible deberá separarse:

**identidad del usuario**

de

**contexto necesario para generar el viaje.**

---

## 35. IA y datos personales

Antes de utilizar información personal dentro de procesos de IA deberá preguntarse:

> ¿La IA realmente necesita conocer este dato?

Por ejemplo, para recomendar una ruta normalmente no será necesario conocer:

- documento de identidad;
- dirección particular;
- información bancaria;
- contraseña.

La minimización deberá mantenerse también dentro del Engine.

---

## 36. Entrenamiento y datos

ZAREVOA deberá definir claramente si determinados datos pueden utilizarse para:

- analítica;
- mejora del producto;
- evaluación del Engine;
- entrenamiento de sistemas propios.

Cuando corresponda deberá aplicarse consentimiento, anonimización u otra base legal adecuada.

La finalidad deberá comunicarse claramente.

---

## 37. Anonimización

Cuando sea posible, los análisis internos deberán utilizar información anonimizada o agregada.

Ejemplo:

Para analizar si los viajes de siete días tienen demasiadas bases, normalmente no será necesario conocer la identidad del usuario.

---

## 38. Pseudonimización

Cuando la anonimización completa no sea posible podrá utilizarse pseudonimización.

Esto permitirá separar identificadores directos de los datos utilizados para determinados procesos.

No deberá confundirse pseudonimización con anonimización completa.

---

## 39. Analítica

Las herramientas de analítica deberán configurarse para recopilar únicamente información necesaria.

Deberán evitarse prácticas invasivas sin justificación.

El sistema deberá priorizar métricas de producto y negocio que permitan mejorar ZAREVOA.

---

## 40. Cookies

Cuando se utilicen cookies deberá distinguirse entre:

- esenciales;
- funcionales;
- analíticas;
- publicitarias.

Las obligaciones de consentimiento deberán aplicarse según las jurisdicciones correspondientes.

El usuario deberá recibir información comprensible.

---

## 41. Publicidad

Si ZAREVOA utiliza publicidad digital, deberá evitar compartir información sensible del Travel Profile con plataformas publicitarias sin una base legítima y transparente.

La personalización interna del viaje no deberá convertirse automáticamente en perfilado publicitario externo.

---

## 42. Datos de pago

ZAREVOA deberá minimizar el manejo directo de información financiera sensible.

Cuando sea posible deberá utilizarse un proveedor especializado de pagos.

La plataforma no deberá almacenar números completos de tarjetas si no existe una necesidad y capacidad de cumplimiento específica.

---

## 43. Tokenización de pagos

Cuando el proveedor lo permita deberán utilizarse tokens u otros mecanismos que eviten almacenar directamente credenciales de pago.

Esto reducirá significativamente el riesgo.

---

## 44. PCI y obligaciones de pago

La integración de pagos deberá diseñarse considerando los estándares y obligaciones aplicables al procesamiento de tarjetas.

La arquitectura deberá intentar reducir el alcance de cumplimiento utilizando proveedores especializados.

---

## 45. Afiliados

Cuando el usuario sea derivado hacia un socio externo deberá comprender que abandonará o interactuará con un servicio diferente.

ZAREVOA deberá distinguir claramente:

- plataforma propia;
- proveedor externo;
- relación comercial.

Los terceros tendrán sus propias políticas de privacidad y seguridad.

---

## 46. Compartición de datos

Los datos personales no deberán compartirse con terceros sin:

- necesidad;
- finalidad;
- base legal;
- protección adecuada.

Cuando un proveedor necesite información para prestar un servicio deberá compartirse únicamente lo necesario.

---

## 47. Venta de datos

El modelo económico de ZAREVOA no deberá depender de vender información personal de viajeros.

La confianza deberá tener prioridad sobre posibles ingresos derivados de explotación innecesaria de datos.

---

## 48. Política de privacidad

Antes del lanzamiento público deberá existir una política de privacidad clara.

Deberá explicar, según corresponda:

- qué información se recopila;
- por qué;
- cómo se utiliza;
- con quién se comparte;
- cuánto se conserva;
- derechos del usuario;
- contacto;
- transferencias internacionales;
- cookies.

El lenguaje deberá ser comprensible.

---

## 49. Términos de uso

También deberán existir términos que definan la relación entre usuario y ZAREVOA.

Entre otros aspectos podrán abordar:

- funcionamiento del servicio;
- limitaciones;
- cuentas;
- pagos;
- propiedad intelectual;
- terceros;
- responsabilidad;
- uso permitido.

Estos documentos deberán recibir revisión legal antes de una operación comercial significativa.

---

## 50. Consentimiento

Cuando el consentimiento sea la base utilizada deberá ser:

- informado;
- específico;
- comprensible;
- verificable;
- revocable cuando corresponda.

No deberá utilizarse una aceptación genérica para justificar cualquier uso futuro de información.

---

## 51. Derechos del usuario

Según la jurisdicción, los usuarios podrán tener derechos relacionados con:

- acceso;
- corrección;
- eliminación;
- oposición;
- limitación;
- portabilidad.

ZAREVOA deberá construir procesos que permitan responder adecuadamente a estas solicitudes.

---

## 52. Eliminación de cuenta

El usuario deberá disponer de un procedimiento claro para solicitar la eliminación de su cuenta.

La eliminación deberá considerar:

- información activa;
- viajes;
- datos personales;
- backups;
- obligaciones legales;
- información que deba conservarse legítimamente.

No deberá prometerse eliminación instantánea absoluta si existen copias técnicas temporales o obligaciones legales que impidan hacerlo.

---

## 53. Retención de datos

Cada categoría de información deberá tener una política de conservación.

La pregunta será:

> ¿Durante cuánto tiempo necesitamos realmente este dato?

Los datos no deberán mantenerse indefinidamente por defecto.

---

## 54. Historial de viajes

El historial puede aportar valor al usuario y mejorar personalización.

Sin embargo, deberá existir control sobre:

- almacenamiento;
- eliminación;
- acceso;
- reutilización.

La conservación deberá estar vinculada a una finalidad legítima.

---

## 55. Exportación

En etapas posteriores podrá ofrecerse al usuario capacidad de descargar o exportar información relacionada con su cuenta y viajes.

Esto puede mejorar:

- control;
- portabilidad;
- confianza.

La función deberá evitar exponer información de otros usuarios.

---

## 56. Registro de actividad

Las acciones sensibles podrán generar registros internos.

Ejemplos:

- inicio de sesión;
- cambios de seguridad;
- acceso administrativo;
- eliminación;
- modificación de permisos;
- operaciones críticas.

Los registros también deberán protegerse.

---

## 57. Logs

Los logs técnicos no deberán convertirse accidentalmente en repositorios de información personal.

Deberá evitarse registrar innecesariamente:

- contraseñas;
- tokens;
- datos financieros;
- contenido sensible;
- información completa del Travel Profile cuando no sea necesaria.

---

## 58. Monitoreo

ZAREVOA deberá supervisar progresivamente:

- errores;
- accesos anormales;
- fallos de autenticación;
- tráfico sospechoso;
- consumo inesperado;
- problemas de proveedores.

El objetivo será detectar incidentes lo antes posible.

---

## 59. Alertas de seguridad

Determinados eventos deberán generar alertas.

Ejemplos:

- múltiples intentos de acceso;
- cambios administrativos;
- exposición de secretos;
- actividad anormal;
- aumento inesperado de errores;
- posible acceso cruzado.

Los umbrales deberán ajustarse según experiencia.

---

## 60. Gestión de vulnerabilidades

Las vulnerabilidades deberán clasificarse según:

- severidad;
- exposición;
- probabilidad;
- impacto;
- facilidad de explotación.

Los problemas críticos deberán recibir tratamiento prioritario.

---

## 61. Actualizaciones

Los componentes críticos deberán mantenerse actualizados.

Las actualizaciones deberán probarse antes de producción cuando exista riesgo de regresión.

Seguridad y estabilidad deberán gestionarse conjuntamente.

---

## 62. Incidentes de seguridad

ZAREVOA deberá contar con un procedimiento básico de respuesta.

La secuencia será:

**Detectar**

↓

**Contener**

↓

**Investigar**

↓

**Corregir**

↓

**Recuperar**

↓

**Comunicar**

↓

**Aprender**

La velocidad será importante, pero también la precisión.

---

## 63. Clasificación de incidentes

Podrán existir niveles como:

### Crítico

Exposición significativa de datos, compromiso administrativo o afectación grave.

### Alto

Acceso no autorizado limitado o vulnerabilidad importante.

### Medio

Problema con impacto controlado.

### Bajo

Evento menor sin evidencia de compromiso.

La clasificación deberá adaptarse conforme crezca la plataforma.

---

## 64. Responsable del incidente

Incluso con un equipo pequeño deberá existir claridad sobre quién coordina un incidente.

La persona responsable deberá:

- centralizar información;
- coordinar acciones;
- evitar cambios contradictorios;
- registrar decisiones;
- controlar comunicación.

---

## 65. Comunicación de incidentes

Cuando un incidente afecte a usuarios deberá comunicarse conforme a:

- impacto;
- evidencia disponible;
- obligaciones legales;
- riesgo.

La comunicación deberá evitar tanto ocultamiento como especulación.

---

## 66. Notificación legal

Determinadas jurisdicciones pueden exigir notificar incidentes de datos dentro de plazos específicos.

ZAREVOA deberá conocer las obligaciones aplicables a sus mercados.

Cuando corresponda deberá buscarse asesoría especializada.

---

## 67. Postmortem

Después de un incidente importante deberá realizarse una revisión.

Deberá responder:

- qué ocurrió;
- por qué ocurrió;
- qué impacto tuvo;
- cómo se detectó;
- cómo se resolvió;
- qué controles faltaban;
- qué se modificará.

El objetivo será evitar repetición.

---

## 68. Seguridad de administradores

Las cuentas administrativas deberán recibir protección reforzada.

Deberán utilizar:

- credenciales únicas;
- autenticación multifactor cuando sea posible;
- mínimo privilegio;
- dispositivos seguros;
- registro de accesos.

Una cuenta administrativa comprometida puede tener un impacto muy superior a una cuenta normal.

---

## 69. Acceso de desarrolladores

El acceso directo a producción deberá limitarse.

Cuando sea posible deberán existir procesos controlados para:

- despliegues;
- consultas;
- cambios;
- recuperación.

No todos los desarrolladores necesitarán acceso completo a datos reales.

---

## 70. Colaboradores externos

Freelancers, agencias o proveedores deberán recibir únicamente los accesos necesarios.

Al terminar una relación deberán revocarse:

- cuentas;
- claves;
- tokens;
- permisos;
- accesos a repositorios.

Este proceso deberá formar parte del cierre de colaboración.

---

## 71. Seguridad del dominio

El dominio principal de ZAREVOA será un activo crítico.

Deberá protegerse mediante:

- contraseña robusta;
- MFA;
- datos de recuperación actualizados;
- bloqueo de transferencia cuando corresponda;
- renovación automática;
- acceso limitado.

La pérdida del dominio podría afectar toda la empresa.

---

## 72. Seguridad del correo corporativo

Las cuentas de correo asociadas a:

- administración;
- pagos;
- dominio;
- proveedores;
- soporte;

deberán tener protección reforzada.

El correo suele ser una vía principal para recuperar otras cuentas.

---

## 73. Ingeniería social

No todos los ataques serán técnicos.

ZAREVOA deberá estar preparada frente a:

- phishing;
- solicitudes falsas;
- suplantación;
- enlaces maliciosos;
- recuperación fraudulenta de cuentas.

La capacitación será parte de la seguridad cuando exista equipo.

---

## 74. Gestión de dispositivos

Los dispositivos utilizados para administrar ZAREVOA deberán mantener:

- actualizaciones;
- bloqueo;
- protección de acceso;
- cifrado cuando sea posible;
- copias de seguridad apropiadas.

Un equipo comprometido puede proporcionar acceso a múltiples sistemas.

---

## 75. Continuidad y seguridad

El plan de seguridad deberá coordinarse con el plan de continuidad.

Un ataque no solo puede exponer información.

También puede impedir operar.

Por ello deberán existir procedimientos para:

- recuperar;
- restaurar;
- cambiar credenciales;
- aislar sistemas;
- mantener funciones críticas.

---

## 76. Dependencia de proveedores

Para cada proveedor crítico deberá conocerse:

- qué datos procesa;
- qué función cumple;
- qué ocurre si falla;
- cómo se reemplaza;
- cómo se revoca el acceso.

Esto reducirá riesgos de dependencia.

---

## 77. Transferencias internacionales

Una plataforma internacional puede procesar información en diferentes países.

ZAREVOA deberá conocer progresivamente:

- dónde se almacenan datos;
- dónde se procesan;
- qué proveedores participan;
- qué mecanismos legales aplican.

Este análisis será especialmente importante al expandirse internacionalmente.

---

## 78. Regulación

ZAREVOA deberá identificar las normas de privacidad aplicables según:

- ubicación empresarial;
- ubicación de usuarios;
- mercados objetivo;
- tipo de información;
- proveedores.

La estrategia deberá revisarse antes de expansiones relevantes.

---

## 79. GDPR y otras normativas

Si ZAREVOA atiende mercados donde resulte aplicable, deberá evaluar requisitos de marcos como GDPR y otras leyes de privacidad.

No deberá utilizarse una única política genérica suponiendo que cubre automáticamente todas las jurisdicciones.

La implementación definitiva deberá recibir revisión jurídica especializada cuando corresponda.

---

## 80. Registro de proveedores

Deberá mantenerse progresivamente un inventario de terceros.

Para cada proveedor:

- nombre;
- finalidad;
- datos procesados;
- ubicación;
- acceso;
- criticidad;
- contrato;
- fecha de revisión.

Esto permitirá comprender el ecosistema de datos.

---

## 81. Inventario de datos

ZAREVOA deberá saber qué información posee.

Podrá mantenerse un inventario con:

- categoría;
- finalidad;
- ubicación;
- responsable;
- retención;
- proveedor;
- sensibilidad.

No puede protegerse correctamente aquello cuya existencia se desconoce.

---

## 82. Clasificación de información

Podrán definirse categorías como:

### Pública

Información destinada a publicación.

### Interna

Información operacional.

### Confidencial

Información comercial o de usuarios.

### Restringida

Información de alta sensibilidad.

Los controles deberán aumentar según clasificación.

---

## 83. Desarrollo seguro

Las nuevas funciones deberán revisar:

- entradas;
- permisos;
- errores;
- datos;
- dependencias;
- secretos;
- logs.

Las funciones críticas deberán recibir mayor revisión antes de producción.

---

## 84. Revisión de código

Cuando el equipo crezca, los cambios sensibles deberán recibir revisión por otra persona antes de producción cuando sea posible.

Esto puede reducir:

- errores;
- vulnerabilidades;
- cambios accidentales.

---

## 85. Automatización de seguridad

Podrán utilizarse progresivamente herramientas para detectar:

- secretos expuestos;
- dependencias vulnerables;
- configuraciones incorrectas;
- errores de código;
- actividad sospechosa.

La automatización deberá complementar la revisión humana.

---

## 86. Pruebas de seguridad

Antes de etapas importantes deberán realizarse pruebas sobre:

- autenticación;
- autorización;
- sesiones;
- APIs;
- cuentas;
- datos;
- pagos.

Con el crecimiento podrán incorporarse evaluaciones externas especializadas.

---

## 87. Programa de vulnerabilidades

En una etapa más madura podrá evaluarse un canal formal para recibir reportes responsables de vulnerabilidades.

Deberá indicar:

- cómo reportar;
- qué información incluir;
- qué sistemas están incluidos;
- cómo responderá ZAREVOA.

No será obligatorio implementar un programa complejo durante la V1.

---

## 88. Seguridad y experiencia

Las medidas de seguridad no deberán hacer innecesariamente difícil utilizar ZAREVOA.

La solución deberá buscar:

**máxima protección razonable con mínima fricción innecesaria.**

Los controles más estrictos deberán concentrarse donde exista mayor riesgo.

---

## 89. Seguridad y crecimiento

El crecimiento aumenta:

- usuarios;
- datos;
- pagos;
- proveedores;
- colaboradores;
- exposición.

Por ello la seguridad deberá evolucionar junto con el negocio.

Una arquitectura suficiente para cien usuarios puede no ser suficiente para cien mil.

---

## 90. Checklist mínimo antes de la V1

Antes del lanzamiento público deberá comprobarse al menos:

- HTTPS activo;
- autenticación segura;
- autorización por usuario;
- secretos fuera del código;
- base de datos protegida;
- backups;
- validación de entradas;
- logs sin datos sensibles innecesarios;
- política de privacidad;
- términos;
- proveedores identificados;
- proceso de eliminación;
- monitoreo básico;
- procedimiento de incidentes.

Este será un mínimo, no el estado final.

---

## 91. Prioridad de riesgos

Durante la V1 deberán priorizarse especialmente riesgos relacionados con:

1. acceso a cuentas;
2. exposición de viajes;
3. secretos;
4. base de datos;
5. pagos;
6. pérdida de información;
7. proveedores externos;
8. abuso de APIs;
9. cuentas administrativas.

La seguridad deberá enfocarse primero donde el impacto potencial sea mayor.

---

## 92. Métricas de seguridad

Podrán observarse:

- intentos fallidos de acceso;
- incidentes;
- vulnerabilidades abiertas;
- tiempo de corrección;
- errores de autorización;
- disponibilidad;
- fallos de backups;
- accesos administrativos.

Las métricas deberán utilizarse para reducir riesgo.

---

## 93. Revisión periódica

La seguridad deberá revisarse:

- antes de lanzamientos importantes;
- al incorporar pagos;
- al incorporar nuevos proveedores;
- al entrar en nuevos mercados;
- después de incidentes;
- periódicamente durante operación.

La seguridad no será una tarea que se complete una sola vez.

---

## 94. Confianza del usuario

La privacidad deberá comunicarse de forma comprensible.

El usuario deberá poder entender:

- qué sabe ZAREVOA sobre él;
- para qué lo utiliza;
- qué puede controlar;
- cómo puede eliminarlo.

La confianza no deberá depender únicamente de documentos legales extensos.

---

## 95. Seguridad como ventaja

Una buena protección puede convertirse en parte de la propuesta de confianza.

ZAREVOA manejará información relacionada con viajes futuros.

Esa información merece protección especial.

El usuario deberá sentir que puede planificar sin perder control sobre sus datos.

---

## 96. Lo que ZAREVOA no deberá hacer

ZAREVOA deberá evitar:

- recopilar datos sin finalidad;
- almacenar contraseñas en texto plano;
- exponer claves en GitHub;
- compartir información innecesariamente;
- vender datos personales;
- dar acceso interno ilimitado;
- guardar información indefinidamente;
- utilizar datos sensibles para publicidad sin justificación;
- ocultar incidentes importantes;
- depender exclusivamente de IA para decisiones de seguridad.

---

## 97. Responsabilidad compartida

La seguridad dependerá de:

**Tecnología**

+

**Procesos**

+

**Personas**

+

**Proveedores**

+

**Usuarios.**

Ninguna herramienta por sí sola garantizará protección completa.

---

## 98. Evolución

La estrategia deberá crecer junto con ZAREVOA.

### V1

Controles fundamentales.

### Crecimiento inicial

Mayor monitoreo, roles y automatización.

### Expansión

Cumplimiento internacional y controles avanzados.

### Escala

Gobernanza formal, auditorías y especialización.

La complejidad deberá aumentar cuando el riesgo lo justifique.

---

## 99. Resultado esperado

Este plan deberá permitir que ZAREVOA pueda:

- proteger cuentas;
- proteger viajes;
- reducir exposición de datos;
- controlar accesos;
- responder a incidentes;
- cumplir progresivamente obligaciones;
- trabajar con proveedores de forma segura;
- crecer sin perder control.

La seguridad deberá acompañar la evolución del producto.

---

## 100. Principio final

La información del viajero no deberá considerarse simplemente un recurso para mejorar algoritmos.

Pertenece al ámbito personal del usuario y deberá tratarse con respeto.

La regla será:

**Recopilar menos.**

**Proteger mejor.**

**Utilizar con propósito.**

**Conservar solo lo necesario.**

**Dar control al usuario.**

---

## 101. Cierre

La confianza será uno de los activos más importantes de ZAREVOA.

Un viajero podrá entregar información sobre:

- dónde quiere ir;
- cuándo viajará;
- con quién;
- cuánto quiere gastar;
- qué le interesa.

ZAREVOA deberá demostrar que merece esa confianza.

La seguridad y la privacidad no serán únicamente requisitos técnicos o legales.

Serán parte de la experiencia y de la identidad de la marca.

**Seguridad + Privacidad + Transparencia + Control = Confianza.**

**ZAREVOA — PLAN YOUR WORLD**
