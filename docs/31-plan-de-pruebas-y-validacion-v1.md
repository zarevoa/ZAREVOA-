# ZAREVOA — Plan de Pruebas y Validación V1

## 1. Objetivo

Este documento define el plan oficial de pruebas y validación de ZAREVOA V1 antes de su lanzamiento público.

El objetivo no será únicamente comprobar que la plataforma funciona técnicamente.

ZAREVOA deberá demostrar que puede generar planes de viaje:

- Coherentes.
- Realistas.
- Personalizados.
- Logísticamente viables.
- Compatibles con el presupuesto.
- Adaptados al ritmo del viajero.
- Fáciles de comprender y modificar.

La validación deberá realizarse progresivamente, desde pruebas internas hasta pruebas con usuarios reales.

---

## 2. Principio general

Una funcionalidad no se considerará validada únicamente porque no produzca errores técnicos.

También deberá comprobarse que produzca un resultado útil.

Por ejemplo:

Un itinerario puede generarse correctamente desde el punto de vista técnico y, aun así, ser incorrecto si incluye demasiadas actividades, desplazamientos absurdos o decisiones incompatibles con el Travel Profile.

Por esta razón, las pruebas deberán evaluar tanto:

**Funcionamiento técnico**

como

**Calidad de planificación**

---

## 3. Etapas de prueba

La validación de ZAREVOA V1 se dividirá en cinco etapas principales:

### Etapa 1 — Pruebas de componentes

Validación individual de funcionalidades.

### Etapa 2 — Pruebas del ZAREVOA Engine

Validación de reglas y decisiones de planificación.

### Etapa 3 — Pruebas de viajes completos

Simulación del proceso completo de principio a fin.

### Etapa 4 — Beta cerrada

Pruebas con un grupo reducido de usuarios reales.

### Etapa 5 — Validación previa al lanzamiento

Revisión final antes de abrir ZAREVOA públicamente.

---

# A. PRUEBAS FUNCIONALES

## 4. Registro y acceso

Comprobar:

- [ ] Creación de cuenta.
- [ ] Inicio de sesión.
- [ ] Cierre de sesión.
- [ ] Recuperación de acceso.
- [ ] Persistencia de sesión.
- [ ] Protección de información entre usuarios.

Resultado esperado:

Cada usuario deberá acceder únicamente a su propia información y recuperar correctamente sus viajes guardados.

---

## 5. Travel Profile

Crear múltiples perfiles de prueba.

Comprobar:

- [ ] Creación.
- [ ] Guardado.
- [ ] Edición.
- [ ] Recuperación.
- [ ] Aplicación de preferencias.
- [ ] Cambio de preferencias.

Resultado esperado:

Dos Travel Profiles significativamente diferentes deberán producir diferencias reales en las recomendaciones cuando el destino y las fechas sean iguales.

---

## 6. Formulario de viaje

Probar:

- [ ] Campos obligatorios.
- [ ] Campos opcionales.
- [ ] Fechas válidas.
- [ ] Fechas incorrectas.
- [ ] Duraciones cortas.
- [ ] Duraciones largas.
- [ ] Presupuesto.
- [ ] Número de viajeros.
- [ ] Ritmo.
- [ ] Intereses.
- [ ] Preferencias.

El sistema deberá explicar claramente cualquier información faltante o incorrecta.

---

# B. PRUEBAS DEL ZAREVOA ENGINE

## 7. Objetivo del motor

El ZAREVOA Engine deberá ser evaluado como un sistema de decisiones.

No bastará con comprobar que genera contenido.

Las pruebas deberán responder:

**¿La decisión que tomó ZAREVOA tiene sentido para este viajero y este viaje?**

---

## 8. Número de bases

Crear viajes con distintas duraciones.

Ejemplos de prueba:

- 3 días.
- 5 días.
- 7 días.
- 10 días.
- 14 días.
- 21 días.

Evaluar:

- [ ] Número de bases.
- [ ] Noches por base.
- [ ] Distancias.
- [ ] Valor real de cada cambio.
- [ ] Exceso de desplazamientos.

El motor deberá evitar convertir un viaje corto en una sucesión constante de hoteles y transportes.

---

## 9. Prueba de estabilidad de base

Crear un escenario donde existan varias ciudades cercanas que puedan visitarse como excursión.

Comprobar si ZAREVOA:

- [ ] Mantiene una base cuando resulta razonable.
- [ ] Propone excursiones cuando corresponde.
- [ ] Evita cambios de alojamiento innecesarios.

Resultado esperado:

El sistema deberá valorar el costo real de cambiar de alojamiento y no únicamente la distancia entre ciudades.

---

## 10. Ritmo Relajado

Crear itinerarios con ritmo Relajado.

Evaluar:

- [ ] Número de actividades diarias.
- [ ] Tiempo libre.
- [ ] Distancias.
- [ ] Pausas.
- [ ] Hora aproximada de inicio y término.

Resultado esperado:

El viajero deberá poder disfrutar el día sin sensación de carrera constante.

---

## 11. Ritmo Equilibrado

Evaluar:

- [ ] Actividades principales.
- [ ] Tiempo de desplazamiento.
- [ ] Descanso.
- [ ] Flexibilidad.

Resultado esperado:

Deberá existir un equilibrio razonable entre aprovechamiento del destino y comodidad.

---

## 12. Ritmo Intenso

Evaluar:

- [ ] Mayor aprovechamiento del día.
- [ ] Viabilidad real.
- [ ] Tiempo suficiente para cada actividad.
- [ ] Traslados.
- [ ] Límites físicos razonables.

Resultado esperado:

Intenso deberá significar mayor actividad, no un itinerario imposible.

---

# C. PRUEBAS DE TRANSICIONES

## 13. Vuelo de llegada

Crear escenarios con llegada:

- [ ] Por la mañana.
- [ ] Al mediodía.
- [ ] Por la tarde.
- [ ] Por la noche.
- [ ] Muy tarde.

Evaluar si ZAREVOA ajusta correctamente las actividades del primer día.

---

## 14. Vuelo de salida

Crear escenarios con vuelos:

- [ ] Muy temprano.
- [ ] Por la mañana.
- [ ] Por la tarde.
- [ ] Por la noche.

El sistema deberá reservar tiempo suficiente para:

- Traslado.
- Procesos previos al vuelo.
- Margen razonable.

---

## 15. Cambio de ciudad

Probar desplazamientos mediante:

- [ ] Avión.
- [ ] Tren.
- [ ] Autobús.
- [ ] Vehículo.
- [ ] Ferry cuando corresponda.

Comprobar que ZAREVOA considere el tiempo total de transición y no únicamente el tiempo anunciado del transporte principal.

---

## 16. Día parcialmente perdido

Crear un traslado que consuma gran parte del día.

Resultado esperado:

ZAREVOA deberá reducir automáticamente las actividades previstas para esa jornada.

---

# D. PRUEBAS DE PRESUPUESTO

## 17. Nivel Económico

Evaluar:

- [ ] Tipo de alojamiento recomendado.
- [ ] Transporte.
- [ ] Actividades.
- [ ] Distribución del presupuesto.
- [ ] Coherencia general.

No deberá interpretarse “económico” como una experiencia necesariamente incómoda o de baja calidad.

---

## 18. Nivel Equilibrado

Comprobar que el presupuesto se distribuya razonablemente entre:

- Alojamiento.
- Transporte.
- Alimentación.
- Actividades.
- Otros gastos.

---

## 19. Nivel Confort

Comprobar que el aumento de presupuesto se utilice donde realmente pueda mejorar la experiencia.

No deberá simplemente aumentar todos los gastos automáticamente.

---

## 20. Nivel Premium

Evaluar:

- [ ] Calidad de opciones.
- [ ] Conveniencia.
- [ ] Ubicación.
- [ ] Experiencias.
- [ ] Transporte.

Premium deberá representar valor y comodidad, no simplemente seleccionar las opciones más caras.

---

## 21. Presupuesto insuficiente

Crear deliberadamente viajes donde el presupuesto sea poco realista.

Resultado esperado:

ZAREVOA no deberá fingir que el viaje es viable.

Deberá explicar el problema y proponer alternativas como:

- Reducir duración.
- Cambiar alojamiento.
- Modificar transporte.
- Reducir actividades pagadas.
- Cambiar determinadas bases.
- Ajustar el presupuesto.

---

# E. PRUEBAS DE PERSONALIZACIÓN

## 22. Perfil cultural

Crear un viajero con fuerte interés en:

- Historia.
- Museos.
- Arquitectura.
- Cultura.

Comprobar que las recomendaciones reflejen realmente esos intereses.

---

## 23. Perfil naturaleza

Crear un perfil orientado a:

- Paisajes.
- Parques.
- Senderismo.
- Naturaleza.

Comparar el resultado con el perfil cultural utilizando el mismo destino.

---

## 24. Perfil gastronómico

Evaluar si el itinerario deja espacio razonable para:

- Gastronomía.
- Mercados.
- Barrios.
- Experiencias culinarias.

No deberá añadir simplemente restaurantes de forma genérica.

---

## 25. Perfil mixto

Crear viajeros con varios intereses.

Resultado esperado:

El itinerario deberá equilibrarlos sin intentar incluir absolutamente todo.

---

# F. MUST SEE Y FOR YOU

## 26. Must See

Comprobar:

- [ ] Relevancia real.
- [ ] Compatibilidad con tiempo disponible.
- [ ] Ubicación.
- [ ] Ausencia de exceso de lugares obligatorios.

Un Must See no deberá incluirse automáticamente si destruye la lógica completa del viaje.

---

## 27. For You

Crear varios perfiles para un mismo destino.

Resultado esperado:

Las recomendaciones For You deberán cambiar de manera perceptible según el Travel Profile.

---

# G. PRUEBAS POR TIPO DE VIAJERO

## 28. Viajero individual

Evaluar:

- [ ] Ritmo.
- [ ] Transporte.
- [ ] Actividades.
- [ ] Flexibilidad.

---

## 29. Pareja

Comprobar que las recomendaciones respondan a intereses declarados y no a suposiciones automáticas sobre lo que una pareja debería hacer.

---

## 30. Familia

Probar familias con distintas composiciones.

Evaluar:

- [ ] Logística.
- [ ] Ritmo.
- [ ] Distancias.
- [ ] Actividades.
- [ ] Descanso.

---

## 31. Grupo de amigos

Crear preferencias parcialmente diferentes.

Evaluar si el sistema consigue un equilibrio razonable.

---

## 32. Diferentes edades

Crear perfiles con edades distintas pero intereses iguales.

Resultado esperado:

La edad podrá influir cuando sea relevante, pero no deberá sustituir las preferencias declaradas.

---

# H. PRUEBAS DE RUTA RECOMENDADA

## 33. Presentación

Comprobar que “Tu ruta recomendada” permita entender rápidamente:

- [ ] Dónde dormirá el usuario.
- [ ] Cuántas noches.
- [ ] En qué orden.
- [ ] Cómo se trasladará.
- [ ] Por qué se recomienda esa estructura.

---

## 34. Añadir base

El usuario añade una ciudad.

Comprobar:

- [ ] Recalculo.
- [ ] Noches.
- [ ] Traslados.
- [ ] Presupuesto.
- [ ] Viabilidad.

---

## 35. Eliminar base

Comprobar que el sistema reorganice correctamente el resto de la ruta.

---

## 36. Cambiar noches

Mover una noche de una ciudad a otra.

Resultado esperado:

El itinerario posterior deberá respetar la nueva distribución.

---

# I. PRUEBAS DE MODIFICACIÓN

## 37. Cambio de actividad

Solicitar:

“Esta actividad no me interesa.”

Comprobar que ZAREVOA:

- [ ] La elimine.
- [ ] Proponga alternativa relevante cuando corresponda.
- [ ] Mantenga coherencia horaria.
- [ ] No regenere innecesariamente todo el viaje.

---

## 38. Cambio de ritmo

Cambiar de Intenso a Relajado después de generar el itinerario.

Resultado esperado:

El sistema deberá reducir carga de actividades y reorganizar únicamente lo necesario.

---

## 39. Cambio de presupuesto

Reducir significativamente el presupuesto.

Evaluar cómo ZAREVOA adapta las recomendaciones.

---

## 40. Cambio de intereses

Añadir un nuevo interés durante la planificación.

Comprobar que las nuevas recomendaciones reflejen el cambio sin perder toda la estructura ya aprobada.

---

# J. PRUEBAS DE DATOS

## 41. Información actualizada

Cuando ZAREVOA utilice datos externos, comprobar:

- [ ] Fuente correcta.
- [ ] Fecha o actualidad cuando sea relevante.
- [ ] Manejo de datos faltantes.
- [ ] Manejo de contradicciones.
- [ ] Diferenciación entre dato y estimación.

---

## 42. Precios

Los precios variables deberán mostrarse como estimaciones cuando no exista información confirmada en tiempo real.

ZAREVOA nunca deberá presentar una estimación como una garantía.

---

## 43. Horarios

Cuando un horario sea importante para la viabilidad del itinerario, deberá utilizarse información confiable o indicarse claramente que necesita verificación.

---

# K. PRUEBAS DE IA

## 44. Consistencia

Repetir varias veces escenarios iguales o muy similares.

Evaluar:

- [ ] Coherencia.
- [ ] Variaciones razonables.
- [ ] Respeto de reglas.
- [ ] Ausencia de contradicciones importantes.

---

## 45. Alucinaciones

Buscar activamente casos donde la IA pueda inventar:

- Lugares.
- Horarios.
- Servicios.
- Precios.
- Distancias.
- Eventos.

Registrar cada caso y determinar cómo evitar su repetición.

---

## 46. Instrucciones contradictorias

Ejemplo:

Usuario solicita:

- Presupuesto muy bajo.
- Hoteles de lujo.
- Muchas ciudades.
- Pocos días.
- Ritmo relajado.

Resultado esperado:

ZAREVOA deberá detectar el conflicto y ayudar a priorizar.

No deberá fingir que todas las condiciones pueden cumplirse simultáneamente.

---

# L. PRUEBAS DE INTERFAZ

## 47. Móvil

Probar dispositivos y tamaños diferentes.

Evaluar:

- [ ] Legibilidad.
- [ ] Botones.
- [ ] Formularios.
- [ ] Mapas.
- [ ] Itinerarios largos.
- [ ] Navegación.
- [ ] Modificaciones.

---

## 48. Escritorio

Comprobar:

- [ ] Aprovechamiento del espacio.
- [ ] Legibilidad.
- [ ] Navegación.
- [ ] Consistencia con móvil.

---

## 49. Accesibilidad básica

Revisar:

- [ ] Contraste.
- [ ] Tamaño de texto.
- [ ] Navegación clara.
- [ ] Etiquetas de formularios.
- [ ] Mensajes de error.

---

# M. PRUEBAS DE RENDIMIENTO

## 50. Tiempo de respuesta

Medir:

- [ ] Carga inicial.
- [ ] Guardado.
- [ ] Generación de ruta.
- [ ] Generación de itinerario.
- [ ] Modificación.
- [ ] Consultas externas.

Definir posteriormente objetivos concretos según la infraestructura seleccionada.

---

## 51. Operaciones largas

Cuando una generación tarde más de lo esperado:

- [ ] Mostrar estado.
- [ ] Evitar doble envío.
- [ ] Manejar timeout.
- [ ] Permitir recuperación cuando sea posible.

---

# N. PRUEBAS DE FALLOS

## 52. API externa caída

Simular fallo de un proveedor.

Resultado esperado:

La plataforma deberá continuar cuando sea posible o explicar claramente la limitación.

---

## 53. IA no disponible

Comprobar:

- [ ] Manejo del error.
- [ ] Reintento controlado cuando corresponda.
- [ ] Mensaje comprensible.
- [ ] No pérdida del trabajo del usuario.

---

## 54. Pérdida de conexión

Simular interrupción durante:

- Formulario.
- Generación.
- Modificación.

Siempre que sea posible, el usuario deberá conservar la información ya introducida.

---

# O. PRUEBAS DE SEGURIDAD

## 55. Acceso entre usuarios

Intentar acceder a viajes pertenecientes a otra cuenta.

Resultado esperado:

Acceso denegado.

---

## 56. Entradas inesperadas

Probar:

- Campos excesivamente largos.
- Caracteres especiales.
- Entradas incompletas.
- Datos mal formados.

El sistema deberá validar y manejar correctamente estas situaciones.

---

## 57. Credenciales y claves

Comprobar que:

- [ ] No existen claves API en frontend.
- [ ] No existen secretos en repositorios públicos.
- [ ] Variables sensibles están protegidas.
- [ ] Logs no muestran información crítica.

---

# P. MATRIZ DE VIAJES DE PRUEBA

## 58. Casos mínimos

Antes del lanzamiento deberán probarse, como mínimo:

### Caso 1
3 días — una ciudad — viajero individual — Económico — Intenso.

### Caso 2
5 días — pareja — Equilibrado — intereses culturales.

### Caso 3
7 días — familia — Confort — ritmo Relajado.

### Caso 4
10 días — varias ciudades — Equilibrado — presupuesto definido.

### Caso 5
14 días — viaje internacional — múltiples bases — Equilibrado.

### Caso 6
21 días — ruta compleja — varios tipos de transporte.

### Caso 7
Presupuesto deliberadamente insuficiente.

### Caso 8
Demasiadas ciudades para el tiempo disponible.

### Caso 9
Llegada nocturna y salida temprana.

### Caso 10
Cambio importante después de aprobar la ruta.

Cada caso deberá conservarse como escenario reutilizable para futuras versiones.

---

# Q. REGISTRO DE RESULTADOS

## 59. Ficha de prueba

Cada error relevante deberá registrar:

- Identificador.
- Fecha.
- Versión.
- Escenario.
- Resultado esperado.
- Resultado obtenido.
- Severidad.
- Evidencia cuando corresponda.
- Estado.
- Responsable.
- Fecha de corrección.

---

## 60. Severidad

Los problemas podrán clasificarse como:

### Crítico

Impide utilizar una función esencial, compromete seguridad o genera resultados peligrosamente incorrectos.

### Alto

Afecta significativamente la calidad del viaje o una función importante.

### Medio

Existe un problema visible, pero el usuario puede continuar.

### Bajo

Problema menor, visual o de poca influencia sobre el resultado.

---

## 61. Prioridad de corrección

Antes del lanzamiento:

- [ ] Todos los críticos deberán estar resueltos.
- [ ] Los problemas altos deberán resolverse salvo excepción documentada.
- [ ] Los problemas medios deberán evaluarse.
- [ ] Los problemas bajos podrán incorporarse al backlog.

---

# R. BETA CERRADA

## 62. Objetivo

La beta deberá comprobar algo que las pruebas internas no pueden demostrar completamente:

**¿Una persona que no participó en el diseño entiende ZAREVOA y consigue crear un viaje útil sin ayuda constante?**

---

## 63. Selección de usuarios

La beta deberá incluir, cuando sea posible, distintos tipos de viajeros:

- Viajeros frecuentes.
- Viajeros ocasionales.
- Personas que planifican mucho.
- Personas que normalmente no planifican.
- Diferentes edades.
- Diferentes presupuestos.
- Diferentes estilos de viaje.

---

## 64. Qué observar

Durante las pruebas deberá observarse:

- Dónde dudan.
- Qué preguntas no comprenden.
- Qué intentan pulsar.
- Qué modifican.
- Qué recomendaciones rechazan.
- Qué partes valoran.
- Dónde abandonan.

La observación del comportamiento puede ser más útil que preguntar únicamente si “les gustó”.

---

## 65. Preguntas posteriores

Después de completar un viaje podrán utilizarse preguntas como:

- ¿Entendiste por qué ZAREVOA recomendó esta ruta?
- ¿Sentiste que el viaje estaba pensado para ti?
- ¿Cambiarías algo importante?
- ¿Hubo alguna recomendación que no tuviera sentido?
- ¿Te pareció demasiado cargado o demasiado vacío?
- ¿Confiarías en utilizar este itinerario en un viaje real?
- ¿Volverías a utilizar ZAREVOA?

---

# S. CRITERIOS DE VALIDACIÓN

## 66. Validación funcional

La plataforma deberá completar correctamente el flujo principal sin errores críticos.

---

## 67. Validación de calidad

Las rutas deberán superar revisión humana en aspectos como:

- Lógica geográfica.
- Tiempo.
- Ritmo.
- Personalización.
- Presupuesto.
- Transiciones.

---

## 68. Validación de usuario

Los usuarios beta deberán poder comprender y utilizar el producto sin asistencia permanente.

---

## 69. Validación técnica

La infraestructura deberá demostrar estabilidad suficiente para la escala inicial prevista.

---

## 70. Validación económica

Deberá conocerse aproximadamente el costo técnico de:

- Crear un usuario.
- Generar una ruta.
- Generar un itinerario.
- Realizar modificaciones.

Esto permitirá evitar lanzar un modelo cuyo costo de operación sea desconocido.

---

# T. DECISIÓN FINAL

## 71. GO

ZAREVOA V1 podrá avanzar al lanzamiento cuando:

- El flujo principal sea estable.
- No existan errores críticos abiertos.
- El ZAREVOA Engine genere rutas razonables de forma consistente.
- Las transiciones sean realistas.
- El presupuesto funcione suficientemente bien.
- La personalización sea perceptible.
- Las modificaciones funcionen.
- La experiencia móvil sea adecuada.
- La información del usuario esté protegida.
- Los usuarios beta puedan utilizar la plataforma.

---

## 72. NO-GO

El lanzamiento deberá detenerse si:

- Existen problemas graves de seguridad.
- Se pierden viajes o información.
- El motor genera frecuentemente rutas imposibles.
- Los días de traslado son sistemáticamente irreales.
- La personalización no funciona.
- Existen fallos frecuentes en el flujo principal.
- El usuario no puede comprender cómo utilizar la plataforma.

---

## 73. Validación continua

Las pruebas no terminarán con el lanzamiento.

Cada cambio importante del ZAREVOA Engine deberá volver a comprobar los escenarios principales.

La matriz de viajes de prueba deberá convertirse progresivamente en una herramienta permanente de control de calidad.

Cuando se corrija un error importante, deberá añadirse una prueba que ayude a evitar que ese mismo problema reaparezca.

---

## 74. Principio final

La calidad de ZAREVOA no se medirá por la cantidad de texto que pueda generar la inteligencia artificial.

Se medirá por la calidad de las decisiones que ayude a tomar.

Antes de lanzar V1, la pregunta fundamental deberá ser:

**“¿Confiaríamos realmente en realizar este viaje siguiendo el plan que ZAREVOA acaba de crear?”**

Si la respuesta es sí de forma consistente en escenarios diversos, ZAREVOA estará acercándose al nivel necesario para salir al mercado.

---

**Estado del documento:** Plan oficial de pruebas y validación de ZAREVOA V1.
