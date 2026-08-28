141 — PROTOCOLO DE CONTINUIDAD OPERACIONAL ZAREVOA V1

1. Objetivo

Establecer criterios básicos para mantener ZAREVOA operativa ante fallos tecnológicos, indisponibilidad de proveedores, errores de infraestructura u otras situaciones que puedan afectar temporalmente el servicio.

El objetivo será proteger la continuidad de las funciones esenciales y reducir el impacto sobre los viajeros.

2. Principio general

ZAREVOA dependerá de diferentes componentes propios y externos.

Por ello, la plataforma deberá diseñarse progresivamente evitando que un fallo no esencial provoque la caída completa del servicio.

La prioridad será mantener disponible el núcleo:

acceso → Travel Profile → ruta → itinerario → viajes guardados.

3. Funciones críticas

Se considerarán especialmente importantes:

- Acceso a la plataforma.
- Autenticación cuando corresponda.
- Recuperación de viajes.
- Travel Profile.
- ZAREVOA Engine.
- Generación y consulta de rutas.
- Generación y consulta de itinerarios.
- Base de datos.
- Servicios esenciales de infraestructura.

4. Dependencias

Antes del lanzamiento deberán identificarse las principales dependencias externas, incluyendo según corresponda:

- Hosting.
- Base de datos.
- Inteligencia artificial.
- Mapas.
- APIs de lugares.
- Autenticación.
- Pagos.
- Correo.
- Analítica.
- Afiliados y reservas.

Para cada dependencia deberá conocerse qué parte de ZAREVOA deja de funcionar si el servicio falla.

5. Fallo parcial

Siempre que sea técnicamente razonable, el fallo de una función secundaria no deberá impedir utilizar el resto de la plataforma.

Por ejemplo, una indisponibilidad temporal de un proveedor de reservas no debería necesariamente impedir consultar un itinerario ya guardado.

6. Viajes guardados

Los viajes previamente creados deberán protegerse especialmente.

Cuando sea posible, una interrupción temporal de servicios de generación no deberá impedir consultar información ya almacenada que siga siendo válida.

7. Proveedores externos

Para servicios críticos deberá evaluarse progresivamente:

- Fiabilidad.
- Historial de disponibilidad.
- Límites.
- Costos.
- Dependencia.
- Alternativas existentes.
- Facilidad de sustitución.

No será necesario disponer desde V1 de un proveedor alternativo para cada servicio, pero sí conocer los puntos de dependencia importantes.

8. Inteligencia artificial

Si el proveedor de IA no se encuentra disponible, ZAREVOA deberá evitar generar respuestas incompletas o engañosas.

Según la función afectada podrá:

- Informar temporalmente la indisponibilidad.
- Permitir consultar viajes existentes.
- Conservar el Travel Profile.
- Permitir reintentar posteriormente.

9. Mapas y datos externos

Cuando fallen fuentes de distancias, ubicaciones u horarios, el sistema deberá evitar sustituir automáticamente esos datos por información inventada.

Si no puede realizar una planificación suficientemente fiable, deberá comunicarlo claramente.

10. Pagos

Un fallo del proveedor de pagos deberá aislarse del resto del producto cuando sea posible.

La plataforma podrá continuar ofreciendo funciones no dependientes del cobro mientras se resuelve el problema.

Nunca deberá considerarse exitoso un pago sin confirmación fiable del proveedor correspondiente.

11. Base de datos

La base de datos será una dependencia crítica.

Deberán existir medidas apropiadas para:

- Respaldo.
- Recuperación.
- Control de acceso.
- Monitoreo.
- Migraciones.
- Protección frente a eliminación accidental.

12. Infraestructura

La infraestructura deberá seleccionarse considerando:

- Disponibilidad.
- Capacidad de recuperación.
- Escalabilidad razonable.
- Seguridad.
- Costos adecuados para V1.

No será necesario diseñar desde el comienzo una arquitectura para millones de usuarios si todavía no existe esa necesidad.

13. Degradación controlada

Cuando una función no esté disponible, será preferible mantener parcialmente operativo el producto antes que provocar una caída completa.

Ejemplos:

- Consultar itinerarios aunque temporalmente no puedan regenerarse.
- Guardar cambios localmente cuando sea técnicamente seguro y sincronizarlos posteriormente.
- Desactivar temporalmente una integración secundaria.

14. Mensajes al usuario

Cuando exista una interrupción, los mensajes deberán explicar:

- Qué función está temporalmente afectada.
- Si la información ya guardada continúa disponible.
- Si puede reintentarse.
- Qué alternativa existe cuando corresponda.

Se evitarán mensajes técnicos incomprensibles.

15. Respaldo

Los datos críticos deberán contar con mecanismos de respaldo adecuados.

La frecuencia y retención deberán ajustarse al crecimiento y volumen real de la plataforma.

16. Recuperación

Se deberán definir progresivamente procedimientos para recuperar:

- Aplicación.
- Configuración.
- Base de datos.
- Documentación técnica.
- Credenciales mediante sistemas seguros.

La recuperación deberá probarse; no bastará con asumir que un respaldo funciona.

17. Prioridad de recuperación

Ante una interrupción amplia, el orden general será:

1. Seguridad y protección de datos.
2. Acceso a información ya guardada.
3. Funciones principales de planificación.
4. Pagos y funciones comerciales.
5. Funciones secundarias.

El orden podrá modificarse según el incidente concreto.

18. Objetivos de recuperación

Durante V1 no será necesario establecer compromisos empresariales complejos de disponibilidad.

Sin embargo, a medida que crezca el producto deberán definirse objetivos como:

- Tiempo máximo deseado de recuperación.
- Cantidad máxima aceptable de información que podría perderse ante un fallo grave.

Estos objetivos deberán basarse en necesidades reales y capacidad tecnológica.

19. Pruebas de continuidad

Periódicamente deberán simularse situaciones como:

- API externa caída.
- Proveedor de IA no disponible.
- Error de base de datos.
- Fallo durante despliegue.
- Pérdida temporal de conectividad.
- Restauración desde respaldo.

20. Documentación

Las dependencias, procedimientos de recuperación y decisiones de continuidad deberán mantenerse actualizados cuando cambie la arquitectura.

21. Evolución

La continuidad operacional deberá crecer junto con ZAREVOA.

Una V1 con pocos usuarios podrá utilizar mecanismos relativamente simples.

Una plataforma con miles de usuarios, pagos y reservas necesitará controles más avanzados, automatización y redundancia.

22. Resultado esperado

ZAREVOA deberá ser capaz de enfrentar fallos razonables sin perder innecesariamente información ni convertir cada problema de un proveedor en una interrupción total.

23. Principio final

La continuidad no significa garantizar que nada falle.

Significa diseñar ZAREVOA para que, cuando algo falle, el impacto sea limitado, la información esté protegida y el servicio pueda recuperarse de manera ordenada.
