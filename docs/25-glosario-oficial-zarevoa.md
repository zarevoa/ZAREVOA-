# ZAREVOA — Glosario Oficial

## 1. Propósito

Este documento define los términos principales utilizados dentro de ZAREVOA.

Su objetivo es mantener un lenguaje consistente entre:

- Documentación.
- Producto.
- Diseño.
- Desarrollo.
- Marketing.
- Atención al usuario.
- Futuras integraciones y colaboradores.

Cuando un término tenga una definición específica dentro de ZAREVOA, esta deberá utilizarse como referencia.

---

## 2. ZAREVOA

**ZAREVOA** es la marca principal y la plataforma de planificación de viajes.

Su propósito es comprender cómo quiere viajar una persona y transformar sus preferencias, restricciones y contexto en una ruta e itinerario coherentes, realistas y personalizados.

ZAREVOA no se define únicamente como un generador de itinerarios.

---

## 3. PLAN YOUR WORLD

**PLAN YOUR WORLD** es la expresión asociada a la identidad de ZAREVOA.

Representa la idea de que cada viajero puede construir una forma propia de descubrir el mundo.

Su utilización deberá mantenerse coherente con la identidad visual y verbal de la marca.

---

## 4. Travel Profile

El **Travel Profile** es el conjunto estructurado de información que permite a ZAREVOA comprender cómo desea viajar una persona.

Puede considerar:

- Destino.
- Fechas.
- Duración.
- Presupuesto.
- Ritmo.
- Intereses.
- Composición del grupo.
- Preferencias.
- Prioridades.
- Restricciones declaradas.

El Travel Profile constituye una de las principales entradas del ZAREVOA Engine.

---

## 5. ZAREVOA Engine

El **ZAREVOA Engine** es el motor de planificación de la plataforma.

Su arquitectura conceptual combina:

**Datos reales + reglas propias ZAREVOA + inteligencia artificial.**

Su función es transformar la información del Travel Profile y los datos disponibles en decisiones de planificación.

---

## 6. ZAREVOA Engine V1

**ZAREVOA Engine V1** es la primera versión funcional del motor.

Deberá encargarse inicialmente de decisiones como:

- Selección de bases.
- Distribución de días.
- Ritmo del viaje.
- Tiempos de transición.
- Coherencia geográfica.
- Presupuesto.
- Priorización de intereses.
- Selección de recomendaciones.
- Construcción de la ruta.
- Apoyo a la generación del itinerario.

V1 representa el núcleo inicial y podrá evolucionar posteriormente.

---

## 7. Reglas ZAREVOA

Las **Reglas ZAREVOA** son criterios propios utilizados por el Engine para tomar o validar decisiones.

Ejemplos:

- Evitar demasiados cambios de alojamiento.
- Reducir actividades en días de traslado.
- Considerar tiempo real de transición.
- Adaptar la cantidad de actividades al ritmo.
- Evaluar la coherencia entre presupuesto y ruta.
- Priorizar intereses declarados.

Estas reglas permiten que ZAREVOA mantenga un criterio propio y no dependa completamente de una IA.

---

## 8. Datos reales

Dentro de ZAREVOA, **datos reales** son datos obtenidos de fuentes adecuadas y utilizados para respaldar decisiones de planificación.

Pueden incluir:

- Ubicaciones.
- Distancias.
- Tiempos.
- Transporte.
- Horarios.
- Precios.
- Clima.
- Información de lugares.

Cuando un dato sea estimado o pueda cambiar, deberá comunicarse apropiadamente.

---

## 9. Inteligencia artificial / IA

La **inteligencia artificial** es una herramienta utilizada dentro del ZAREVOA Engine para interpretar, personalizar y generar información.

La IA no constituye por sí sola el sistema de planificación.

Deberá trabajar junto con datos reales y reglas ZAREVOA.

---

## 10. Base

Una **base** es una ciudad, localidad o zona donde el viajero se aloja durante una parte relevante del viaje y desde la cual puede realizar actividades o excursiones.

Ejemplo:

Una persona puede utilizar Florencia como base durante cuatro noches y realizar desde allí diferentes visitas.

ZAREVOA deberá evitar crear bases innecesarias.

---

## 11. Cambio de base

Un **cambio de base** ocurre cuando el viajero deja un alojamiento en una ciudad o zona y se traslada a otra donde establecerá una nueva base.

No deberá evaluarse únicamente por la duración del transporte.

También implica tiempo y esfuerzo asociado al proceso completo de traslado.

---

## 12. Tiempo de transición

El **tiempo de transición** representa el tiempo real asociado a desplazarse entre etapas importantes del viaje.

Puede incluir:

- Preparación.
- Check-out.
- Traslado al punto de salida.
- Espera.
- Transporte.
- Equipaje.
- Traslado al nuevo alojamiento.
- Check-in.
- Margen razonable.

Es un concepto fundamental para evitar itinerarios poco realistas.

---

## 13. Día de transición

Un **día de transición** es una jornada que incluye un traslado significativo, vuelo, tren importante o cambio de base.

ZAREVOA deberá reducir normalmente la cantidad de actividades planificadas para estas jornadas.

---

## 14. Ruta

La **ruta** representa la estructura geográfica principal del viaje.

Define:

- Destinos.
- Bases.
- Orden.
- Distribución general de días.

La ruta se define antes de generar el itinerario detallado.

---

## 15. Tu ruta recomendada

**Tu ruta recomendada** es la etapa de ZAREVOA en la que el usuario visualiza la estructura propuesta para su viaje antes de generar el itinerario completo.

Permitirá comprender:

- Bases.
- Orden.
- Número de noches o días.
- Estructura general.

El usuario podrá aprobarla o modificarla.

---

## 16. Itinerario

El **itinerario** es la planificación detallada del viaje después de que la ruta principal haya sido definida o aprobada.

Puede incluir:

- Actividades.
- Lugares.
- Desplazamientos.
- Recomendaciones.
- Organización diaria.
- Información práctica.

El itinerario deberá respetar las decisiones establecidas en el Travel Profile y la ruta.

---

## 17. Ritmo de viaje

El **ritmo de viaje** define el nivel general de intensidad de la planificación.

ZAREVOA utilizará inicialmente tres niveles:

### Relajado

Menor cantidad de actividades, más pausas y mayor margen.

### Equilibrado

Balance entre actividades, desplazamientos y tiempo libre.

### Intenso

Mayor aprovechamiento de la jornada manteniendo límites realistas.

---

## 18. Nivel de presupuesto

El **nivel de presupuesto** es una forma simplificada de indicar el estilo económico esperado del viaje.

Inicialmente:

- Económico.
- Equilibrado.
- Confort.
- Premium.

Podrá complementarse con un presupuesto total definido directamente por el usuario.

---

## 19. Presupuesto definido

El **presupuesto definido** es una cantidad económica concreta indicada por el viajero para el viaje.

ZAREVOA deberá utilizarla como una restricción o referencia real de planificación y no únicamente como información descriptiva.

---

## 20. Must See

**Must See** identifica lugares o experiencias especialmente relevantes dentro de un destino.

No significa que sean obligatorios.

Representa aquellas experiencias que, por su importancia, singularidad o relevancia, ZAREVOA considera que vale la pena destacar.

---

## 21. For You

**For You** identifica recomendaciones seleccionadas específicamente por su relación con el Travel Profile.

Su objetivo es hacer visible la personalización.

Dos viajeros en el mismo destino podrán recibir recomendaciones For You diferentes.

---

## 22. Recomendación

Una **recomendación** es una opción que ZAREVOA considera adecuada para el viajero según el contexto de su planificación.

Puede ser:

- Destino.
- Base.
- Actividad.
- Experiencia.
- Transporte.
- Alojamiento.
- Otro elemento relevante.

Una recomendación no necesita generar ingresos para ZAREVOA.

---

## 23. Opción reservable

Una **opción reservable** es una alternativa que el usuario puede reservar o comprar mediante un proveedor.

Puede coincidir con una recomendación, pero ambos conceptos deberán mantenerse separados.

---

## 24. Afiliado

Un **afiliado** es un proveedor o programa comercial mediante el cual ZAREVOA puede recibir una comisión cuando un usuario realiza una acción o reserva elegible.

La existencia de una comisión no deberá determinar artificialmente la recomendación.

---

## 25. Recomendación genuina

Una **recomendación genuina** es aquella seleccionada por su utilidad para el viajero y no únicamente por existir una oportunidad de monetización.

Es uno de los principios comerciales fundamentales de ZAREVOA.

---

## 26. ZAREVOA Journey

**ZAREVOA Journey** es un producto o nivel de servicio orientado a ofrecer una experiencia de planificación más completa y personalizada.

Sus funcionalidades exactas deberán definirse según la evolución y validación del producto.

No deberá prometer servicios que no puedan entregarse de manera consistente.

---

## 27. ZAREVOA Personal

**ZAREVOA Personal** es un nivel de servicio con mayor intervención o acompañamiento humano.

Podrá utilizarse para viajeros que requieran un nivel adicional de personalización, revisión o apoyo en determinadas decisiones.

Su alcance deberá mantenerse claramente definido.

---

## 28. Acompañamiento ZAREVOA

**Acompañamiento ZAREVOA** es el concepto utilizado para describir el apoyo adicional que pueda ofrecerse dentro de determinados productos o servicios.

No implica automáticamente atención permanente ni disponibilidad 24/7.

El alcance dependerá del producto contratado.

---

## 29. V1

**V1** significa primera versión funcional de ZAREVOA.

Su objetivo será validar el núcleo del producto sin intentar incorporar desde el inicio todas las funcionalidades futuras.

El flujo esencial será:

**Travel Profile → ZAREVOA Engine → Tu ruta recomendada → modificación → aprobación → itinerario.**

---

## 30. MVP

**MVP — Minimum Viable Product** o **Producto Mínimo Viable** es una versión suficientemente funcional para probar la propuesta principal con usuarios reales.

Dentro de ZAREVOA, el concepto deberá interpretarse como:

**la versión más pequeña capaz de demostrar correctamente el valor central del producto.**

Mínimo no significa incompleto ni de mala calidad.

---

## 31. Backlog

El **backlog** es el registro de funcionalidades, mejoras e ideas que podrían desarrollarse posteriormente.

Una idea dentro del backlog no está automáticamente aprobada para desarrollo.

Deberá priorizarse según evidencia, impacto, coste y coherencia con ZAREVOA.

---

## 32. KPI

**KPI — Key Performance Indicator** o **Indicador Clave de Rendimiento** es una métrica utilizada para evaluar el desempeño de un área importante del producto o negocio.

Ejemplos:

- Travel Profiles completados.
- Rutas generadas.
- Itinerarios completados.
- Usuarios recurrentes.
- Conversión comercial.

---

## 33. Planificación útil completada

Una **planificación útil completada** es una de las métricas centrales propuestas para ZAREVOA V1.

Inicialmente representa un flujo en el que el usuario:

1. Completa la información necesaria.
2. Recibe una ruta.
3. La aprueba o modifica.
4. Obtiene un itinerario.

Con el tiempo podrán incorporarse señales adicionales de utilidad.

---

## 34. Usuario recurrente

Un **usuario recurrente** es una persona que vuelve a ZAREVOA después de una utilización anterior.

Especialmente relevante será el usuario que regrese para crear un nuevo viaje.

Esto podrá considerarse una señal importante de confianza en el producto.

---

## 35. Coste por planificación

El **coste por planificación** representa el coste tecnológico aproximado necesario para generar y mantener un viaje.

Puede considerar:

- IA.
- APIs.
- Mapas.
- Infraestructura.
- Procesamiento.
- Almacenamiento.

Será una métrica importante para evaluar la sostenibilidad económica de ZAREVOA.

---

## 36. Integración

Una **integración** es la conexión de ZAREVOA con un servicio o proveedor externo.

Ejemplos:

- Mapas.
- Transporte.
- Clima.
- Alojamiento.
- Actividades.
- Pagos.
- Afiliados.

Las integraciones deberán diseñarse procurando evitar dependencias innecesarias.

---

## 37. API

**API — Application Programming Interface** es un mecanismo que permite a ZAREVOA intercambiar información o ejecutar funciones mediante servicios externos.

Las APIs podrán proporcionar datos necesarios para el funcionamiento del Engine.

Su consumo, coste, disponibilidad y dependencia deberán ser controlados.

---

## 38. Caché

La **caché** es un mecanismo para almacenar temporalmente información utilizada con frecuencia.

Puede ayudar a:

- Reducir consultas externas.
- Disminuir costes.
- Mejorar velocidad.
- Reducir dependencia inmediata de proveedores.

Su utilización deberá considerar cuánto tiempo continúa siendo válida la información almacenada.

---

## 39. Mobile first

**Mobile first** significa diseñar considerando desde el inicio la experiencia en teléfonos móviles.

No significa ignorar computadores o tablets.

Significa evitar que la versión móvil sea tratada como una adaptación secundaria.

---

## 40. Escalabilidad

La **escalabilidad** es la capacidad de ZAREVOA para aumentar usuarios, destinos, datos, idiomas y funcionalidades sin tener que reconstruir completamente el sistema ni deteriorar significativamente su funcionamiento.

---

## 41. Validación

La **validación** es el proceso de comprobar con evidencia real si las hipótesis de ZAREVOA son correctas.

Ejemplos:

- Si los usuarios entienden el producto.
- Si completan el Travel Profile.
- Si consideran útiles las rutas.
- Si regresan.
- Si están dispuestos a pagar.

La validación deberá preceder a inversiones importantes de crecimiento.

---

## 42. Personalización

Dentro de ZAREVOA, **personalización** significa que la información del viajero produce diferencias reales en las decisiones de planificación.

No deberá limitarse a:

- Cambiar un nombre.
- Reordenar una lista genérica.
- Modificar superficialmente un texto.

La personalización deberá afectar la estructura o contenido del viaje cuando corresponda.

---

## 43. Coherencia

La **coherencia** representa la capacidad de una planificación para mantener sentido en su conjunto.

Incluye:

- Geografía.
- Tiempo.
- Presupuesto.
- Ritmo.
- Intereses.
- Secuencia.
- Transiciones.

Una actividad puede ser buena individualmente y aun así no ser coherente dentro de una ruta determinada.

---

## 44. Transparencia

La **transparencia** es el principio de comunicar de forma clara aquello que pueda afectar la confianza o decisiones del usuario.

Puede incluir:

- Información estimada.
- Datos que deben verificarse.
- Relaciones de afiliados.
- Alcance de servicios.
- Limitaciones.

---

## 45. Principio “Primero recomendación”

**Primero recomendación. Después monetización.**

Es el principio que establece que la utilidad para el viajero deberá determinar primero qué opción tiene sentido recomendar.

La posibilidad de obtener ingresos deberá evaluarse después y no sustituir el criterio de planificación.

---

## 46. Principio maestro ZAREVOA

Ante una decisión importante, ZAREVOA deberá volver a la pregunta:

**¿Esta decisión ayuda a comprender mejor cómo quiere viajar esta persona y a convertirlo en un viaje coherente, realista y personalizado?**

Este principio sirve como referencia para producto, tecnología, diseño y negocio.

---

## 47. Evolución del glosario

Este glosario deberá actualizarse cuando:

- Se cree un nuevo concepto propio.
- Cambie una definición importante.
- Aparezcan nuevos productos.
- Se incorporen términos técnicos relevantes.
- Una palabra pueda generar interpretaciones diferentes.

Las nuevas definiciones deberán mantenerse coherentes con los principios generales de ZAREVOA.

---

## 48. Declaración final

El lenguaje utilizado dentro de ZAREVOA forma parte de la identidad del producto.

Utilizar conceptos consistentes permitirá que diseño, tecnología, negocio y experiencia del usuario evolucionen en la misma dirección.

Este documento será la referencia terminológica oficial del proyecto ZAREVOA.
