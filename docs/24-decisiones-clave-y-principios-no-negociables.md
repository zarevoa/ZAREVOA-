# ZAREVOA — Decisiones Clave y Principios No Negociables

## 1. Propósito

Este documento reúne las decisiones fundamentales que definen ZAREVOA y que deberán mantenerse como referencia durante el diseño, desarrollo y evolución del proyecto.

Su función es evitar que, con el crecimiento del producto, nuevas tecnologías, oportunidades comerciales o decisiones de implementación hagan que ZAREVOA pierda aquello que lo diferencia.

Estos principios podrán perfeccionarse con evidencia real, pero cualquier cambio importante deberá ser consciente, justificado y documentado.

---

## 2. ZAREVOA no será solo un generador de itinerarios

ZAREVOA deberá comprender primero cómo quiere viajar una persona.

El itinerario será el resultado de un proceso que considera:

- Duración.
- Presupuesto.
- Ritmo.
- Intereses.
- Composición del grupo.
- Preferencias.
- Restricciones declaradas.
- Distancias.
- Tiempos reales.
- Lógica geográfica.
- Prioridades del viajero.

El objetivo no será llenar días con actividades.

Será construir un viaje que tenga sentido.

---

## 3. Travel Profile como base

El Travel Profile será una pieza central de ZAREVOA.

Las recomendaciones deberán partir de la información entregada por el viajero y no únicamente de listas genéricas de lugares populares.

Cada pregunta incorporada al Travel Profile deberá cumplir una condición:

**tener una consecuencia real en la planificación.**

Si una pregunta no cambia ninguna decisión relevante, deberá evaluarse si realmente es necesaria.

---

## 4. Arquitectura del ZAREVOA Engine

La arquitectura conceptual aprobada para ZAREVOA Engine V1 será:

**Datos reales + reglas propias ZAREVOA + inteligencia artificial.**

Ninguno de estos elementos deberá reemplazar completamente a los demás.

### Datos reales

Aportarán información verificable sobre lugares, distancias, tiempos, transporte y otras variables necesarias.

### Reglas ZAREVOA

Aportarán estructura, coherencia y criterio propio.

### Inteligencia artificial

Aportará interpretación, flexibilidad, personalización y capacidad de generar respuestas adaptadas.

La IA será una herramienta del Engine.

No será el Engine completo.

---

## 5. Criterio propio ZAREVOA

ZAREVOA deberá desarrollar y conservar criterio propio de planificación.

No deberá limitarse a preguntar a una IA qué viaje recomendar.

Entre las decisiones que deberán estar gobernadas o validadas por reglas ZAREVOA estarán:

- Número razonable de bases.
- Distribución de días.
- Cambios de alojamiento.
- Tiempos de transición.
- Intensidad de las jornadas.
- Coherencia con presupuesto.
- Priorización de intereses.
- Viabilidad general de la ruta.

Esto permitirá construir un producto consistente y diferenciable.

---

## 6. Menos cambios de alojamiento cuando sea razonable

ZAREVOA deberá evitar rutas innecesariamente fragmentadas.

Cambiar de alojamiento consume tiempo y energía.

La selección de bases deberá considerar:

- Duración total.
- Distancias.
- Conectividad.
- Excursiones posibles.
- Valor real de incorporar una nueva base.

Una nueva base deberá justificar suficientemente el esfuerzo que implica.

---

## 7. Tiempo real de transición

ZAREVOA no deberá interpretar un traslado únicamente como el tiempo indicado por un tren, vuelo o automóvil.

Cuando corresponda se considerará:

- Preparación.
- Check-out.
- Traslado al punto de salida.
- Espera.
- Transporte.
- Equipaje.
- Traslado al alojamiento.
- Check-in.
- Margen razonable.

El objetivo será representar mejor el tiempo que realmente pierde o utiliza un viajero durante un cambio de base.

---

## 8. Días de traslado no son días normales

Cuando exista un vuelo, tren importante, cambio de ciudad o traslado significativo, ZAREVOA deberá reducir la carga de actividades.

No se deberán crear itinerarios que técnicamente parezcan posibles pero que en la práctica resulten agotadores o poco realistas.

---

## 9. Ritmos claramente diferenciados

ZAREVOA utilizará inicialmente tres ritmos:

### Relajado

Menor cantidad de actividades, más pausas y mayor margen.

### Equilibrado

Una combinación razonable entre actividades, desplazamientos y tiempo libre.

### Intenso

Mayor cantidad de experiencias y aprovechamiento del día, manteniendo límites realistas.

Seleccionar un ritmo deberá producir diferencias reales en el itinerario.

---

## 10. Presupuesto adaptable

ZAREVOA manejará inicialmente niveles de presupuesto:

- Económico.
- Equilibrado.
- Confort.
- Premium.

También podrá considerar un presupuesto definido directamente por el usuario.

El presupuesto no deberá dividirse mediante porcentajes rígidos para todos los viajes.

La distribución deberá adaptarse según:

- Destino.
- Duración.
- Transporte.
- Intereses.
- Prioridades.
- Estilo de viaje.

---

## 11. El presupuesto debe influir realmente

Solicitar presupuesto y posteriormente ignorarlo sería una falsa personalización.

El ZAREVOA Engine deberá utilizarlo para tomar decisiones.

Cuando una planificación sea claramente incompatible con el presupuesto disponible, ZAREVOA deberá:

- Adaptar.
- Advertir.
- Proponer alternativas.

No deberá simplemente generar un itinerario imposible de financiar.

---

## 12. Intereses ponderados

No todos los intereses deberán tener necesariamente el mismo peso.

ZAREVOA deberá intentar comprender cuáles son realmente prioritarios para el viajero.

Las actividades y recomendaciones deberán reflejar esas prioridades.

---

## 13. “Must See” y “For You”

ZAREVOA distinguirá dos tipos importantes de recomendación:

### Must See

Lugares o experiencias especialmente relevantes dentro del destino.

### For You

Lugares o experiencias recomendados específicamente por su relación con el Travel Profile.

La personalización deberá ser visible para el usuario.

ZAREVOA no deberá limitarse a cambiar el orden de una lista genérica.

---

## 14. Composición del grupo sin estereotipos

La composición y edades del grupo podrán influir en la planificación cuando sean relevantes.

Sin embargo, ZAREVOA no deberá asumir automáticamente que:

- Una persona mayor quiere viajar lentamente.
- Una familia solo quiere actividades infantiles.
- Una pareja quiere actividades románticas.
- Un joven quiere vida nocturna.

Las preferencias declaradas deberán tener prioridad sobre estereotipos.

---

## 15. Tres preguntas antes de recomendar una actividad

Antes de incorporar una actividad al itinerario, ZAREVOA deberá evaluar:

### 1. ¿Le interesa al viajero?

Relación con su Travel Profile.

### 2. ¿Tiene tiempo real para realizarla?

Considerando horarios, desplazamientos y carga del día.

### 3. ¿Tiene sentido dentro de la ruta?

Ubicación, secuencia y contexto.

Una actividad popular no deberá incorporarse automáticamente si falla en estas preguntas.

---

## 16. Primero la ruta, después el detalle

Antes de generar un itinerario completo, ZAREVOA mostrará:

# Tu ruta recomendada

Esta etapa permitirá al usuario comprender:

- Qué bases utilizará.
- Cuántos días permanecerá en cada una.
- Cómo se estructura el viaje.

El usuario deberá poder:

- Aprobar.
- Modificar.

Solo después se generará el itinerario detallado.

---

## 17. Modificar sin comenzar nuevamente

Una decisión fundamental de ZAREVOA será permitir modificar una planificación sin obligar al usuario a repetir todo el Travel Profile.

Si cambia:

- Una ciudad.
- Una base.
- Una cantidad de días.
- El ritmo.
- Un interés.
- Una parte del presupuesto.

El sistema deberá conservar toda la información que continúe siendo válida.

La modificación deberá ser incremental siempre que sea posible.

---

## 18. Recomendación genuina y opción reservable son conceptos distintos

ZAREVOA distinguirá claramente:

### Recomendación

Lo que el sistema considera adecuado para el viajero.

### Opción reservable

Una alternativa que puede comprarse o reservarse mediante un proveedor.

Una recomendación podrá existir aunque ZAREVOA no reciba ninguna comisión.

---

## 19. Monetización después del criterio

La regla comercial fundamental será:

**Primero recomendación. Después monetización.**

Los afiliados, acuerdos comerciales o comisiones no deberán determinar artificialmente qué opción se presenta como mejor.

La confianza del viajero tendrá mayor valor a largo plazo que maximizar una comisión individual.

---

## 20. Transparencia comercial

Cuando ZAREVOA pueda recibir una comisión por una reserva o enlace, deberá comunicarlo de forma apropiada.

El usuario deberá mantener libertad para:

- Utilizar la opción propuesta.
- Comparar.
- Reservar directamente.
- Elegir otro proveedor.

La monetización deberá integrarse sin deteriorar la independencia percibida del planificador.

---

## 21. ZAREVOA Journey y ZAREVOA Personal

ZAREVOA podrá ofrecer diferentes niveles de servicio.

### ZAREVOA Journey

Producto orientado a una experiencia de planificación más completa y personalizada.

### ZAREVOA Personal

Nivel con mayor intervención o acompañamiento humano cuando corresponda.

Estos productos deberán tener límites claros.

ZAREVOA no deberá prometer servicios que no pueda entregar de forma consistente.

---

## 22. Acompañamiento realista

La comunicación comercial deberá utilizar conceptos como:

**Acompañamiento ZAREVOA**

cuando corresponda.

Se evitarán promesas como atención permanente o soporte 24/7 mientras no exista una infraestructura real capaz de proporcionarlo.

La confianza dependerá también de prometer únicamente aquello que puede cumplirse.

---

## 23. Sin estadísticas ficticias

ZAREVOA no utilizará cifras inventadas para aparentar:

- Número de viajeros.
- Viajes creados.
- Países cubiertos.
- Valoraciones.
- Satisfacción.
- Reservas.

Las estadísticas se mostrarán cuando existan datos reales que las respalden.

---

## 24. Diseño con identidad propia

ZAREVOA deberá mantener una identidad visual reconocible.

La marca ZAREVOA tendrá protagonismo y deberá conservar coherencia entre sus diferentes pantallas y productos.

La **Z** podrá utilizarse como elemento visual distintivo de la identidad cuando resulte apropiado.

La estética deberá transmitir:

- Claridad.
- Confianza.
- Viaje.
- Personalización.
- Calidad.

---

## 25. Experiencia global

ZAREVOA se diseñará desde el inicio con capacidad de expansión internacional.

La arquitectura deberá permitir progresivamente:

- Idiomas.
- Monedas.
- Países.
- Zonas horarias.
- Diferentes proveedores.
- Diferentes mercados.

La primera versión podrá tener un alcance limitado sin renunciar a una arquitectura preparada para crecer.

---

## 26. Mobile first en la práctica

Una parte importante de los viajeros utilizará ZAREVOA desde un teléfono.

Por ello, la experiencia móvil no deberá ser una adaptación secundaria de la versión de escritorio.

Formularios, mapas, itinerarios, botones y navegación deberán ser cómodos en pantallas pequeñas.

---

## 27. Datos reales antes que falsa precisión

Cuando ZAREVOA no disponga de información suficientemente confiable, deberá evitar presentar estimaciones como certezas.

Será preferible indicar:

- Aproximación.
- Rango.
- Información pendiente de confirmar.
- Necesidad de verificación.

La apariencia de precisión nunca deberá tener prioridad sobre la honestidad de la información.

---

## 28. Privacidad por diseño

ZAREVOA recopilará únicamente la información necesaria para prestar y mejorar el servicio.

El Travel Profile no deberá convertirse en una recopilación indiscriminada de información personal.

Los usuarios deberán mantener un nivel razonable de control sobre sus datos.

---

## 29. Seguridad desde el inicio

La seguridad no deberá incorporarse únicamente cuando ZAREVOA sea grande.

Desde V1 deberán considerarse:

- Protección de credenciales.
- Claves API.
- Datos personales.
- Control de acceso.
- Dependencias.
- Respaldos.
- Manejo seguro de errores.

Los secretos nunca deberán almacenarse públicamente en el repositorio.

---

## 30. Estructura financiera separada

Antes de activar cobros de ZAREVOA Journey, ZAREVOA Personal o recepción de comisiones de afiliados, se deberá evaluar e implementar una estructura financiera empresarial separada de las finanzas personales.

Inicialmente se evaluará:

- Cuenta empresarial en CLP.
- Cuenta empresarial en USD.
- Recepción de transferencias internacionales.
- Capacidad SWIFT.
- Solución multidivisa internacional cuando sea compatible con la estructura de ZAREVOA.

Esta decisión deberá implementarse antes de una operación comercial significativa.

---

## 31. Construcción progresiva

ZAREVOA no intentará desarrollar desde el inicio todas las funcionalidades imaginadas.

La prioridad de V1 será demostrar el núcleo:

**Travel Profile → ZAREVOA Engine → Tu ruta recomendada → modificación → aprobación → itinerario.**

Las funcionalidades adicionales deberán incorporarse después según evidencia real.

---

## 32. Validar antes de escalar

Antes de realizar inversiones importantes en crecimiento, ZAREVOA deberá comprobar que:

- Los usuarios comprenden el producto.
- Completan la planificación.
- Las rutas son útiles.
- La personalización aporta valor.
- Los usuarios regresan.
- Existe disposición a pagar.

Primero se validará el producto.

Después se acelerará el crecimiento.

---

## 33. Medir utilidad, no solo tráfico

El éxito no se medirá únicamente mediante:

- Visitas.
- Clics.
- Tiempo en pantalla.

ZAREVOA priorizará métricas relacionadas con valor real:

- Travel Profiles completados.
- Rutas generadas.
- Rutas aprobadas.
- Modificaciones.
- Itinerarios completados.
- Usuarios recurrentes.
- Segundo viaje creado.
- Conversión comercial.
- Satisfacción.

---

## 34. Documentar decisiones importantes

Las decisiones relevantes de producto, arquitectura, negocio y experiencia deberán quedar documentadas.

Esto permitirá:

- Mantener coherencia.
- Comprender por qué se tomó una decisión.
- Evitar discusiones repetidas.
- Incorporar colaboradores en el futuro.
- Reducir dependencia de una sola persona.

El repositorio documental será parte de la infraestructura de ZAREVOA.

---

## 35. Una funcionalidad debe justificar su existencia

Antes de desarrollar una nueva función se preguntará:

**¿Esto mejora realmente la planificación del viaje para el usuario?**

Si la respuesta no es clara, la funcionalidad podrá permanecer en el backlog.

Más funciones no significan automáticamente un mejor producto.

---

## 36. La tecnología sirve al viaje

ZAREVOA podrá utilizar:

- Inteligencia artificial.
- APIs.
- Automatización.
- Algoritmos.
- Datos.
- Integraciones.

Pero ninguna tecnología será el objetivo por sí misma.

El usuario no necesita admirar la complejidad tecnológica.

Necesita recibir una planificación que tenga sentido.

---

## 37. Principio maestro

Cuando exista una duda importante sobre producto, tecnología, diseño o negocio, ZAREVOA deberá regresar a una pregunta:

**¿Esta decisión ayuda a comprender mejor cómo quiere viajar esta persona y a convertirlo en un viaje coherente, realista y personalizado?**

Si la respuesta es sí, probablemente está alineada con ZAREVOA.

Si la respuesta es no, deberá existir una razón muy clara para continuar.

---

## 38. Declaración final

ZAREVOA deberá crecer sin perder su esencia.

Su ventaja no será simplemente utilizar inteligencia artificial.

Será combinar tecnología, datos y criterio propio para comprender al viajero y tomar mejores decisiones de planificación.

ZAREVOA deberá ser:

**personal, coherente, realista, transparente y útil.**

Estos principios constituyen la referencia central para las decisiones futuras del proyecto.
