# 59 — Plan de pruebas y control de calidad

## 1. Objetivo

Este documento define el sistema de pruebas y control de calidad de ZAREVOA.

El objetivo será asegurar que cada versión del producto entregue una experiencia:

- estable;
- segura;
- coherente;
- comprensible;
- técnicamente confiable;
- útil para el viajero.

En ZAREVOA, calidad no significará únicamente que la plataforma funcione técnicamente.

También significará que las recomendaciones tengan sentido.

El principio será:

> Una función no estará terminada solamente porque funcione. Estará terminada cuando funcione correctamente para el usuario.

---

## 2. Alcance del control de calidad

El control de calidad deberá cubrir cuatro dimensiones principales:

1. Calidad técnica.
2. Calidad de datos.
3. Calidad de planificación.
4. Calidad de experiencia de usuario.

Las cuatro deberán evaluarse antes de considerar estable una funcionalidad importante.

---

## 3. Calidad técnica

La calidad técnica comprobará que el sistema:

- responda correctamente;
- no genere errores inesperados;
- almacene correctamente la información;
- mantenga la seguridad;
- gestione fallos;
- funcione en diferentes dispositivos;
- mantenga tiempos de respuesta razonables.

---

## 4. Calidad de planificación

Esta será una dimensión especialmente importante para ZAREVOA.

Un itinerario puede ser técnicamente válido y, al mismo tiempo, ser una mala recomendación.

Por ello deberá comprobarse:

- lógica de la ruta;
- número de bases;
- tiempos de traslado;
- ritmo;
- presupuesto;
- intereses;
- carga diaria;
- coherencia geográfica;
- sentido de las actividades.

---

## 5. Calidad de experiencia

Las pruebas deberán comprobar que el usuario comprende:

- qué debe hacer;
- qué información necesita proporcionar;
- qué está haciendo ZAREVOA;
- por qué recibe una recomendación;
- cómo modificarla;
- cómo continuar.

La interfaz deberá reducir incertidumbre y fricción.

---

# ESTRATEGIA DE PRUEBAS

## 6. Niveles de prueba

ZAREVOA utilizará progresivamente:

- pruebas unitarias;
- pruebas de integración;
- pruebas funcionales;
- pruebas end-to-end;
- pruebas de interfaz;
- pruebas de usabilidad;
- pruebas de seguridad;
- pruebas de rendimiento;
- pruebas del Engine;
- pruebas con usuarios reales.

No todas deberán implementarse con el mismo nivel desde el primer día.

---

## 7. Pruebas unitarias

Las pruebas unitarias deberán concentrarse especialmente en lógica que pueda verificarse de manera determinista.

Ejemplos:

- cálculos;
- validaciones;
- reglas;
- presupuesto;
- duración;
- clasificación;
- transformaciones de datos;
- permisos.

Las reglas críticas de ZAREVOA Engine deberán tener una cobertura especialmente cuidadosa.

---

## 8. Pruebas de integración

Deberán comprobar la interacción entre diferentes componentes.

Ejemplos:

**Frontend → Backend**

**Backend → Base de datos**

**Backend → ZAREVOA Engine**

**Engine → IA**

**Backend → APIs externas**

**Pagos → Estado de cuenta**

El objetivo será detectar problemas que no aparecen al probar componentes aisladamente.

---

## 9. Pruebas funcionales

Cada función importante deberá comprobarse desde la perspectiva del usuario.

Ejemplos:

- crear una cuenta;
- completar Travel Profile;
- crear un viaje;
- generar una ruta;
- modificarla;
- aprobarla;
- generar itinerario;
- guardar viaje;
- volver a abrirlo.

---

## 10. Pruebas end-to-end

Deberán simular recorridos completos.

Ejemplo:

**Usuario nuevo**

↓

**Registro**

↓

**Travel Profile**

↓

**Nuevo viaje**

↓

**Tu ruta recomendada**

↓

**Modificación**

↓

**Aprobación**

↓

**Itinerario**

↓

**Guardado**

Estas pruebas serán fundamentales antes de lanzamientos importantes.

---

# PRUEBAS DEL ZAREVOA ENGINE

## 11. Importancia

ZAREVOA Engine necesitará un sistema de evaluación propio.

No bastará comprobar que devuelve una respuesta.

Será necesario comprobar que la respuesta sea razonable.

---

## 12. Casos de referencia

Se creará progresivamente una biblioteca de viajes de prueba.

Cada caso deberá contener:

- duración;
- destinos;
- viajeros;
- presupuesto;
- ritmo;
- intereses;
- restricciones;
- resultado esperado aproximado.

Estos casos permitirán detectar regresiones cuando se modifique el Engine.

---

## 13. Viajes cortos

Se deberán probar viajes de:

- 1 día;
- 2 días;
- 3 días;
- fines de semana.

El Engine deberá evitar rutas excesivamente complejas.

En viajes muy cortos deberá priorizar simplicidad y tiempo útil.

---

## 14. Viajes medios

Se probarán viajes de aproximadamente:

- 4 días;
- 5 días;
- 7 días;
- 10 días.

Deberá comprobarse que el número de bases sea razonable y que exista equilibrio entre actividades y desplazamientos.

---

## 15. Viajes largos

Se probarán viajes de:

- 14 días;
- 21 días;
- 30 días o más.

El sistema deberá poder estructurar viajes extensos sin generar itinerarios repetitivos o innecesariamente intensos.

---

## 16. Una ciudad

Cuando el viaje tenga una única ciudad, el Engine deberá evitar introducir desplazamientos o cambios de alojamiento sin una razón válida.

---

## 17. Varias ciudades

Se probarán combinaciones de múltiples ciudades.

Deberá evaluarse:

- orden;
- distancia;
- transporte;
- noches;
- transición;
- coherencia.

---

## 18. Exceso de destinos

Caso crítico:

Un usuario intenta visitar demasiados destinos en pocos días.

ZAREVOA no deberá obedecer ciegamente.

Deberá advertir el problema y proponer una alternativa más razonable.

---

## 19. Ritmo relajado

Las pruebas deberán comprobar que realmente exista:

- menor número de actividades;
- espacios libres;
- transiciones cómodas;
- menor presión horaria.

---

## 20. Ritmo equilibrado

Deberá existir una combinación razonable de:

- actividades;
- descanso;
- exploración;
- desplazamientos.

---

## 21. Ritmo intenso

Podrá contener más actividades, pero nunca deberá transformarse en un itinerario físicamente imposible.

Intenso no significará irreal.

---

## 22. Días de traslado

Se deberán probar específicamente:

- vuelos;
- trenes;
- buses;
- ferries;
- cambios de alojamiento.

El sistema deberá reducir automáticamente la carga de esos días.

---

## 23. Tiempo real de transición

Las pruebas deberán comprobar que ZAREVOA no utilice solamente el tiempo nominal del transporte.

Ejemplo:

Un vuelo de dos horas no equivale a una transición total de dos horas.

El Engine deberá considerar razonablemente los tiempos asociados.

---

# PRUEBAS DE PRESUPUESTO

## 24. Niveles

Se probarán:

- Económico;
- Equilibrado;
- Confort;
- Premium.

Las diferencias deberán reflejarse realmente en las recomendaciones.

---

## 25. Presupuesto definido

Cuando el usuario introduzca un monto específico, deberá comprobarse que las recomendaciones mantengan coherencia con ese límite.

---

## 26. Presupuesto insuficiente

Si el presupuesto parece incompatible con:

- destino;
- duración;
- número de viajeros;
- nivel esperado;

ZAREVOA deberá indicarlo.

No deberá crear una falsa sensación de viabilidad.

---

## 27. Distribución adaptable

Las pruebas deberán comprobar que el presupuesto no se divida mediante porcentajes rígidos cuando la realidad del viaje requiera otra distribución.

---

# PRUEBAS DE PERSONALIZACIÓN

## 28. Intereses

Se deberán crear perfiles con intereses claramente distintos.

Por ejemplo:

**Perfil A**

- historia;
- museos;
- arquitectura.

**Perfil B**

- naturaleza;
- senderismo;
- gastronomía.

Los itinerarios deberían mostrar diferencias significativas.

---

## 29. Must See y For You

Se comprobará que exista equilibrio entre:

**Must See**

y

**For You.**

El itinerario no deberá ser completamente genérico ni ignorar lugares especialmente relevantes del destino.

---

## 30. Composición del grupo

Se probarán:

- viajero individual;
- pareja;
- familia;
- grupo de amigos;
- grupos multigeneracionales.

El sistema deberá adaptar la planificación sin aplicar estereotipos automáticos.

---

## 31. Preferencias sobre edad

La edad nunca deberá ser suficiente por sí sola para descartar automáticamente una experiencia.

Las preferencias declaradas tendrán mayor importancia.

---

# PRUEBAS DE MODIFICACIÓN

## 32. Modificaciones parciales

Se probarán solicitudes como:

- quitar una actividad;
- cambiar una ciudad;
- agregar una noche;
- reducir actividades;
- aumentar actividades;
- cambiar presupuesto;
- cambiar ritmo.

---

## 33. Conservación del contexto

Cuando el usuario modifique una parte, ZAREVOA deberá conservar las decisiones que no necesitan cambiar.

Ejemplo:

Cambiar una actividad del día 4 no deberá reconstruir innecesariamente todo el viaje.

---

## 34. Modificaciones sucesivas

Se probarán múltiples cambios consecutivos.

El sistema deberá mantener coherencia después de cada modificación.

---

## 35. Conflictos

Si una modificación genera un conflicto, ZAREVOA deberá detectarlo.

Ejemplo:

El usuario elimina una ciudad pero mantiene una actividad ubicada exclusivamente en esa ciudad.

El sistema deberá adaptar la planificación.

---

# PRUEBAS DE DATOS EXTERNOS

## 36. Disponibilidad

Los datos procedentes de terceros pueden:

- cambiar;
- desaparecer;
- contener errores;
- llegar incompletos;
- demorarse.

ZAREVOA deberá manejar estas situaciones sin romper la experiencia completa.

---

## 37. APIs fuera de servicio

Se simularán fallos de proveedores externos.

El sistema deberá responder de manera controlada.

Cuando sea posible deberá:

- mantener el itinerario;
- informar la limitación;
- utilizar información alternativa;
- permitir continuar.

---

## 38. Datos desactualizados

La plataforma deberá evitar presentar como certeza información que pueda haber cambiado.

Esto será especialmente importante para:

- precios;
- horarios;
- disponibilidad;
- restricciones;
- transporte.

---

# PRUEBAS DE INTELIGENCIA ARTIFICIAL

## 39. Variabilidad

Las respuestas generadas por IA pueden variar.

Por ello no todas las pruebas podrán depender de coincidencia textual exacta.

Se evaluarán criterios como:

- coherencia;
- relevancia;
- seguridad;
- precisión;
- cumplimiento de instrucciones;
- tono;
- utilidad.

---

## 40. Alucinaciones

Se crearán casos destinados a comprobar si la IA inventa:

- lugares;
- horarios;
- precios;
- conexiones;
- disponibilidad;
- servicios.

La arquitectura deberá reducir este riesgo utilizando datos reales cuando sean necesarios.

---

## 41. Información no disponible

Cuando ZAREVOA no disponga de información confiable, deberá reconocer la incertidumbre.

Será preferible indicar una limitación antes que inventar una respuesta.

---

## 42. Protección de reglas

Se comprobará que la capa de IA no ignore reglas fundamentales del Engine.

Por ejemplo:

- duración;
- restricciones;
- presupuesto;
- transiciones;
- preferencias.

---

# PRUEBAS DE INTERFAZ

## 43. Dispositivos

La plataforma deberá probarse como mínimo en:

- teléfonos;
- tablets;
- computadores.

La prioridad será la experiencia móvil.

---

## 44. Tamaños de pantalla

Se probarán diferentes resoluciones para evitar:

- textos cortados;
- botones inaccesibles;
- elementos superpuestos;
- desplazamiento innecesario;
- pérdida de información.

---

## 45. Navegadores

Antes de producción deberán comprobarse los navegadores principales utilizados por los usuarios objetivo.

No será necesario garantizar compatibilidad con navegadores obsoletos sin uso significativo.

---

## 46. Formularios

Los formularios deberán probar:

- campos vacíos;
- valores incorrectos;
- caracteres especiales;
- límites;
- navegación;
- mensajes de error;
- recuperación.

Los mensajes deberán explicar cómo corregir el problema.

---

# PRUEBAS DE SEGURIDAD

## 47. Autenticación

Se comprobarán:

- registro;
- acceso;
- cierre de sesión;
- recuperación;
- expiración de sesión;
- protección de rutas.

---

## 48. Autorización

Un usuario no deberá poder acceder a información privada perteneciente a otro usuario.

Esta condición será crítica.

---

## 49. Entradas maliciosas

Las entradas deberán validarse y sanitizarse según corresponda.

Se deberán aplicar buenas prácticas contra vulnerabilidades comunes.

---

## 50. Credenciales

Nunca deberán exponerse públicamente:

- contraseñas;
- claves de API;
- tokens;
- secretos;
- credenciales de proveedores.

GitHub deberá revisarse especialmente para evitar publicación accidental de secretos.

---

## 51. Dependencias

Las dependencias deberán mantenerse actualizadas razonablemente y revisarse ante vulnerabilidades conocidas relevantes.

---

# PRUEBAS DE PAGOS

## 52. Ambiente de pruebas

Los pagos deberán probarse inicialmente en el entorno de pruebas del proveedor.

Nunca se deberán utilizar transacciones reales innecesariamente durante desarrollo.

---

## 53. Escenarios

Se probarán:

- pago exitoso;
- pago rechazado;
- pago pendiente;
- cancelación;
- error;
- reintento;
- reembolso cuando corresponda.

---

## 54. Activación de beneficios

Una compra exitosa deberá activar únicamente los beneficios correspondientes al plan adquirido.

Un pago fallido no deberá activar acceso premium por error.

---

# RENDIMIENTO

## 55. Tiempos de respuesta

Se medirán especialmente:

- carga inicial;
- autenticación;
- guardado;
- generación de ruta;
- modificación;
- generación de itinerario.

---

## 56. Procesos largos

Cuando un proceso no pueda responder inmediatamente, la interfaz deberá comunicar claramente su estado.

El usuario no deberá interpretar una espera normal como un fallo.

---

## 57. Carga

Antes de crecer significativamente deberán realizarse pruebas de carga para comprender:

- capacidad;
- cuellos de botella;
- comportamiento de base de datos;
- consumo de APIs;
- costos de IA.

---

# CONTROL DE REGRESIONES

## 58. Regresión

Cada cambio importante puede romper funciones que anteriormente funcionaban.

Por ello se mantendrá un conjunto creciente de pruebas de regresión.

---

## 59. Casos críticos permanentes

Deberán existir casos que se ejecuten repetidamente antes de versiones importantes.

Entre ellos:

- registro;
- Travel Profile;
- creación de viaje;
- ruta;
- modificación;
- itinerario;
- guardado;
- acceso posterior.

---

## 60. Regresión del Engine

Se conservará una biblioteca de itinerarios de referencia.

Después de modificar reglas o modelos se compararán los resultados.

Una respuesta diferente no será necesariamente un error.

Deberá evaluarse si la nueva respuesta es:

- mejor;
- equivalente;
- peor;
- incoherente.

---

# GESTIÓN DE ERRORES

## 61. Clasificación

Los errores podrán clasificarse inicialmente como:

### Crítico

Impide utilizar el producto o compromete seguridad/datos.

### Alto

Afecta una función principal.

### Medio

Existe una alternativa, pero afecta significativamente la experiencia.

### Bajo

Problema menor o visual.

---

## 62. Prioridad

Los errores críticos deberán resolverse antes de liberar una versión.

Los errores altos deberán evaluarse cuidadosamente antes de producción.

Los problemas cosméticos no deberán bloquear innecesariamente una versión estable.

---

## 63. Registro de errores

Cada error relevante deberá registrar:

- descripción;
- pasos para reproducir;
- resultado esperado;
- resultado obtenido;
- entorno;
- evidencia cuando corresponda;
- severidad;
- estado.

---

## 64. Errores detectados por usuarios

Los reportes reales deberán analizarse para identificar patrones.

Un problema repetido tendrá mayor prioridad que una incidencia aislada de bajo impacto.

---

# VALIDACIÓN CON USUARIOS

## 65. Pruebas piloto

Antes de una apertura amplia se utilizará un grupo controlado de usuarios.

El objetivo será observar comportamiento real.

---

## 66. Observar antes de explicar

Cuando sea posible, deberá observarse si el usuario entiende la interfaz sin recibir instrucciones adicionales.

Si necesita constantemente una explicación, probablemente exista un problema de diseño.

---

## 67. Preguntas de validación

Después de utilizar ZAREVOA será útil conocer:

- ¿La ruta tenía sentido?
- ¿El ritmo fue adecuado?
- ¿Las recomendaciones parecían personales?
- ¿Cambiarías algo?
- ¿Fue fácil modificar el viaje?
- ¿Confiarías en este itinerario?
- ¿Volverías a utilizar ZAREVOA?

---

## 68. Calidad percibida

La calidad técnica no será suficiente.

La pregunta fundamental será:

> ¿El usuario siente que ZAREVOA comprendió cómo quiere viajar?

Esta percepción será una métrica central del producto.

---

# CHECKLIST PREVIO A PRODUCCIÓN

## 69. Funcionalidad

Antes de publicar una versión deberá comprobarse:

- flujo principal operativo;
- formularios;
- navegación;
- Engine;
- guardado;
- modificaciones;
- autenticación.

---

## 70. Seguridad

Comprobar:

- secretos protegidos;
- permisos;
- autenticación;
- conexiones seguras;
- dependencias críticas;
- acceso a datos.

---

## 71. Experiencia

Comprobar:

- móvil;
- textos;
- botones;
- errores;
- tiempos de espera;
- claridad;
- consistencia visual.

---

## 72. Datos

Comprobar:

- almacenamiento;
- recuperación;
- integridad;
- backups;
- tratamiento de errores.

---

## 73. Engine

Comprobar:

- rutas cortas;
- rutas largas;
- múltiples destinos;
- presupuestos;
- ritmos;
- intereses;
- días de transición;
- modificaciones.

---

## 74. Criterio de lanzamiento

No será necesario esperar perfección absoluta.

Sí será necesario que:

- el flujo principal sea estable;
- no existan errores críticos conocidos;
- los datos estén protegidos;
- el Engine entregue resultados razonables;
- el usuario pueda completar el proceso;
- exista capacidad de detectar y corregir problemas.

---

## 75. Mejora continua

El control de calidad continuará después del lanzamiento.

Cada error real deberá convertirse, cuando corresponda, en:

**Problema detectado**

↓

**Corrección**

↓

**Prueba**

↓

**Caso de regresión**

↓

**Aprendizaje**

De esta forma ZAREVOA deberá hacerse progresivamente más confiable.

---

## 76. Principio final

La calidad de ZAREVOA dependerá tanto del software como del criterio de planificación.

Un sistema técnicamente perfecto que produzca malos viajes no será un buen producto.

Un buen itinerario generado por un sistema inestable tampoco será suficiente.

ZAREVOA deberá unir ambos elementos:

**Tecnología confiable + planificación con criterio.**

---

**Estado del documento:** Plan base oficial de pruebas y control de calidad de ZAREVOA.

**Criterio:** probar no solamente que ZAREVOA funcione, sino que sus decisiones sean coherentes, útiles, seguras y confiables para el viajero.
