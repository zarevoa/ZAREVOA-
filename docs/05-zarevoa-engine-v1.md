05 — ZAREVOA Engine V1

Motor de planificación inteligente

ZAREVOA Engine V1 es el núcleo de planificación de ZAREVOA.

Su objetivo es transformar la información entregada por cada viajero en una ruta coherente, personalizada, realista y modificable.

El motor combinará:

- Datos reales del viaje y de los destinos.
- Reglas propias de planificación ZAREVOA.
- Inteligencia artificial.
- Preferencias almacenadas en el Travel Profile.
- Restricciones de tiempo, presupuesto y composición del grupo.

La IA será una herramienta dentro del sistema, pero no reemplazará el criterio de planificación definido por ZAREVOA.

1. Travel Profile

Cada planificación partirá del perfil real del viajero.

El Travel Profile podrá considerar:

- Destino o destinos.
- Fechas del viaje.
- Duración total.
- Número de viajeros.
- Edades o composición del grupo.
- Presupuesto.
- Nivel de comodidad.
- Ritmo de viaje.
- Intereses.
- Actividades prioritarias.
- Preferencias de alojamiento.
- Preferencias de transporte.
- Restricciones o necesidades relevantes.

El objetivo es evitar itinerarios genéricos y adaptar cada viaje a las personas que realmente lo realizarán.

2. Selección inteligente de bases

ZAREVOA no asumirá que visitar más ciudades significa realizar un mejor viaje.

El motor analizará la duración disponible y recomendará bases estratégicas desde las cuales explorar una zona.

Buscará evitar:

- Cambios innecesarios de alojamiento.
- Traslados excesivos.
- Pérdida de tiempo haciendo check-in y check-out.
- Rutas físicamente agotadoras.
- Itinerarios creados únicamente para acumular destinos.

Cuando sea conveniente, recomendará permanecer varias noches en una misma base y realizar excursiones o visitas desde allí.

3. Ritmo de viaje

El usuario podrá elegir inicialmente entre tres ritmos:

Relajado

Menos actividades por día, mayor tiempo libre y desplazamientos más tranquilos.

Equilibrado

Combinación razonable entre actividades, descanso y tiempo disponible.

Intenso

Mayor cantidad de actividades y aprovechamiento del día, siempre dentro de límites realistas.

El ritmo seleccionado afectará directamente la cantidad de actividades propuestas.

4. Tiempo real de transición

ZAREVOA no considerará solamente el tiempo teórico de transporte.

El motor deberá contemplar también:

- Traslado hacia estaciones o aeropuertos.
- Tiempo previo necesario.
- Esperas.
- Recogida de equipaje.
- Traslado al alojamiento.
- Check-in y check-out.
- Pausas razonables.
- Tiempo de adaptación después de un traslado importante.

Los días con vuelos o desplazamientos largos tendrán automáticamente una menor carga de actividades.

5. Presupuesto

ZAREVOA podrá trabajar mediante niveles generales:

- Económico.
- Equilibrado.
- Confort.
- Premium.

También podrá trabajar con un presupuesto definido por el usuario.

El presupuesto no deberá dividirse mediante porcentajes rígidos.

El sistema podrá adaptar la distribución entre:

- Alojamiento.
- Transporte.
- Alimentación.
- Actividades.
- Experiencias.
- Margen para gastos adicionales.

La distribución dependerá del destino, duración, preferencias y prioridades del viajero.

6. Intereses: Must See y For You

ZAREVOA distinguirá entre dos tipos principales de recomendaciones.

Must See

Lugares o experiencias especialmente relevantes dentro del destino.

For You

Recomendaciones seleccionadas específicamente según los intereses y preferencias del viajero.

Esto permitirá combinar los principales atractivos de un destino con experiencias realmente personalizadas.

7. Composición del grupo

El motor tendrá en cuenta quiénes realizan el viaje.

Podrá considerar:

- Viajeros individuales.
- Parejas.
- Familias.
- Grupos de amigos.
- Viajeros de distintas edades.

La edad será un dato contextual y no una regla automática.

ZAREVOA evitará estereotipos y dará prioridad a las preferencias reales declaradas por los viajeros.

8. Criterio para recomendar actividades

Antes de incluir una actividad, ZAREVOA deberá evaluar al menos tres elementos:

1. Si coincide con los intereses del viajero.
2. Si existe tiempo real para realizarla.
3. Si tiene sentido dentro de la ruta propuesta.

Una actividad popular no será incluida automáticamente si perjudica la coherencia general del viaje.

9. Recomendación y monetización

ZAREVOA distinguirá claramente entre:

- Una recomendación genuina.
- Una alternativa reservable.
- Una alternativa que pueda generar una comisión de afiliación.

La posibilidad de obtener una comisión nunca deberá ser el criterio principal para recomendar una opción.

Primero estará la calidad y pertinencia de la recomendación para el viajero.

10. Ruta recomendada antes del itinerario

Antes de generar el itinerario detallado, ZAREVOA mostrará una etapa denominada:

Tu ruta recomendada

Esta pantalla permitirá visualizar la estructura principal del viaje antes de desarrollar todos los días.

El usuario podrá:

- Aprobar la ruta.
- Cambiar destinos.
- Agregar o eliminar una parada.
- Modificar la cantidad de noches.
- Ajustar el ritmo.
- Solicitar alternativas.

Solo después de esta aprobación se generará el itinerario detallado.

11. Modificación sin reiniciar

Una característica fundamental de ZAREVOA será permitir modificar un viaje sin comenzar nuevamente todo el proceso.

Por ejemplo, el usuario podrá indicar:

- Quiero una noche más aquí.
- Elimina esta ciudad.
- Prefiero menos actividades.
- Quiero gastar menos.
- Cambia esta actividad.
- Quiero más naturaleza.
- Prefiero otro alojamiento.

El motor recalculará únicamente las partes afectadas y conservará las decisiones que continúen siendo válidas.

12. Principio central del ZAREVOA Engine

ZAREVOA Engine V1 no buscará generar la mayor cantidad posible de actividades.

Buscará construir el viaje que tenga mayor sentido para cada viajero.

El criterio central será:

Personalización + tiempo real + coherencia de ruta + presupuesto + intereses + flexibilidad.

El resultado esperado es un sistema con criterio propio, humano y útil, capaz de ayudar al viajero a tomar decisiones sin convertir la planificación en un proceso rígido o abrumador.

---

Estado: Arquitectura funcional aprobada para ZAREVOA V1.

Documento: 05-zarevoa-engine-v1.md
