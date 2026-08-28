ZAREVOA — Analítica y Eventos V1

Documento 85


1. Objetivo

Este documento define la estructura inicial de analítica y eventos de ZAREVOA.

El objetivo será comprender cómo utilizan las personas la plataforma, detectar problemas y medir el funcionamiento del producto sin recopilar información innecesaria.

La analítica deberá permitir convertir el comportamiento real de los usuarios en decisiones de mejora.


---

2. Principio de analítica

ZAREVOA medirá aquello que ayude a responder preguntas concretas.

Por ejemplo:

¿Dónde descubren ZAREVOA?

¿Comienzan una planificación?

¿En qué paso abandonan?

¿Completan el Travel Profile?

¿Aceptan o modifican la ruta?

¿Generan el itinerario?

¿Utilizan opciones reservables?

¿Compran Journey o Personal?

¿Regresan para crear otro viaje?

No se recopilarán datos únicamente porque técnicamente sea posible hacerlo.


---

3. Concepto de evento

Un evento representa una acción relevante realizada dentro de ZAREVOA.

Ejemplos:

Usuario inicia planificación.

Usuario completa Travel Profile.

Usuario genera ruta.

Usuario modifica ruta.

Usuario genera itinerario.

Usuario selecciona Journey.

Usuario realiza un pago.

Cada acción podrá registrarse mediante un nombre de evento y determinados atributos necesarios para su análisis.


---

4. Convención de nombres

Los eventos deberán utilizar una convención consistente.

Como referencia técnica podrá utilizarse:

snake_case

Ejemplos:

planning_started

travel_profile_completed

route_generated

route_modified

itinerary_generated

journey_viewed

journey_selected

personal_viewed

personal_selected

checkout_started

purchase_completed

affiliate_link_clicked

La convención definitiva deberá mantenerse igual en toda la plataforma.


---

5. Eventos de adquisición

Podrán registrarse eventos relacionados con la llegada del usuario.

Ejemplos:

landing_page_viewed

content_viewed

planner_cta_clicked

signup_started

signup_completed

También podrán registrarse atributos como:

- Fuente.
- Canal.
- Campaña.
- Página de entrada.
- Idioma.
- Tipo general de dispositivo.

Esto permitirá comprender qué canales generan utilización real.


---

6. Eventos del Travel Profile

El Travel Profile deberá permitir identificar puntos de fricción.

Eventos posibles:

travel_profile_started

travel_profile_step_completed

travel_profile_completed

travel_profile_abandoned

No será necesario enviar como datos analíticos todas las respuestas personales del usuario.

Siempre que sea posible se medirán acciones y categorías generales en lugar de información detallada innecesaria.


---

7. Eventos de ruta

La pantalla “Tu ruta recomendada” tendrá eventos específicos.

Ejemplos:

route_generated

route_viewed

route_approved

route_modified

destination_added

destination_removed

days_distribution_changed

pace_changed

route_regenerated

Estos eventos ayudarán a comprender la calidad inicial de las recomendaciones.


---

8. Eventos del itinerario

Podrán utilizarse:

itinerary_generation_started

itinerary_generated

itinerary_viewed

itinerary_day_viewed

activity_removed

activity_added

activity_replaced

itinerary_saved

itinerary_shared

itinerary_exported

La disponibilidad exacta dependerá de las funciones implementadas en V1.


---

9. Eventos comerciales

Para Journey y Personal podrán medirse:

journey_viewed

journey_selected

personal_viewed

personal_selected

pricing_viewed

checkout_started

checkout_completed

purchase_completed

purchase_failed

refund_requested

refund_completed

Estos eventos permitirán comprender el embudo comercial.


---

10. Eventos de afiliación

Cuando existan opciones reservables podrán registrarse:

bookable_option_viewed

affiliate_link_clicked

booking_provider_selected

Cuando un proveedor permita atribución también podrán incorporarse datos de conversión recibidos posteriormente.

ZAREVOA deberá diferenciar claramente:

Clic.

Reserva.

Comisión confirmada.

No deberán considerarse equivalentes.


---

11. Eventos de retención

Podrán utilizarse eventos como:

user_returned

new_trip_started

travel_profile_reused

previous_trip_viewed

second_trip_created

Esto permitirá analizar la utilización de ZAREVOA entre diferentes viajes.


---

12. Propiedades de eventos

Los eventos podrán contener propiedades que aporten contexto.

Ejemplos:

- Idioma.
- País o mercado general cuando sea apropiado.
- Tipo de dispositivo.
- Duración del viaje.
- Número de viajeros.
- Ritmo seleccionado.
- Nivel general de presupuesto.
- Número de destinos.
- Producto.
- Fuente de adquisición.

Las propiedades deberán limitarse a aquellas necesarias para análisis concretos.


---

13. Identificación de usuarios

Cuando exista una cuenta, ZAREVOA podrá utilizar un identificador interno para relacionar eventos de forma segura.

Las herramientas analíticas no deberán depender innecesariamente de:

- Nombre completo.
- Correo electrónico.
- Teléfono.
- Documentos.
- Direcciones.

Siempre que sea posible se utilizarán identificadores internos o seudónimos.


---

14. Usuarios sin cuenta

Cuando sea legal y técnicamente apropiado, determinadas acciones podrán medirse de forma agregada antes de que exista una cuenta.

Esto permitirá comprender:

- Visitas.
- Inicio de planificación.
- Abandono.
- Rendimiento de páginas.

La implementación deberá respetar las preferencias de privacidad y consentimiento aplicables.


---

15. Datos sensibles

ZAREVOA deberá evitar enviar a herramientas analíticas información sensible o innecesariamente detallada.

Los datos utilizados para generar una planificación no deberán copiarse automáticamente hacia sistemas de analítica.

La información operativa y la información analítica deberán mantenerse separadas cuando sea razonable.


---

16. Embudo principal

Los eventos deberán permitir construir el siguiente embudo:

landing_page_viewed

↓

planning_started

↓

travel_profile_completed

↓

route_generated

↓

route_approved o route_modified

↓

itinerary_generated

↓

journey_selected / personal_selected / affiliate_link_clicked

↓

purchase_completed o conversión atribuida

Este embudo permitirá detectar dónde se produce la mayor pérdida de usuarios.


---

17. Medición de tiempos

Además de eventos podrán medirse tiempos relevantes.

Ejemplos:

- Tiempo para completar Travel Profile.
- Tiempo de generación de ruta.
- Tiempo de generación del itinerario.
- Tiempo hasta primera modificación.
- Tiempo hasta compra.
- Tiempo entre primer y segundo viaje.

Estos indicadores ayudarán a detectar fricción y problemas de rendimiento.


---

18. Errores

Los errores deberán tener una estructura de seguimiento.

Ejemplos:

route_generation_failed

itinerary_generation_failed

payment_failed

api_request_failed

save_failed

Los registros técnicos podrán incluir información necesaria para diagnosticar el problema sin exponer innecesariamente datos personales.


---

19. Rendimiento

ZAREVOA deberá medir aspectos técnicos que afectan directamente la experiencia.

Entre ellos:

- Tiempo de carga.
- Tiempo de respuesta.
- Errores de servidor.
- Fallos de servicios externos.
- Rendimiento móvil.
- Disponibilidad.

La analítica de producto y la observabilidad técnica deberán complementarse.


---

20. Herramientas

La selección definitiva de herramientas de analítica deberá realizarse antes de la implementación.

Se evaluarán criterios como:

- Privacidad.
- Costo.
- Facilidad de integración.
- Embudos.
- Eventos personalizados.
- Paneles.
- Exportación de datos.
- Escalabilidad.
- Cumplimiento normativo.

ZAREVOA deberá evitar incorporar múltiples herramientas que recopilen los mismos datos sin una necesidad clara.


---

21. Panel inicial

Durante V1 deberá existir un panel simple con información esencial.

Podrá incluir:

Visitantes.

Planificaciones iniciadas.

Travel Profiles completados.

Rutas generadas.

Rutas modificadas.

Itinerarios generados.

Conversiones.

Usuarios recurrentes.

Errores principales.

Costo tecnológico por planificación cuando esté disponible.

El panel deberá facilitar decisiones rápidas.


---

22. Alertas

Determinados eventos técnicos podrán generar alertas.

Ejemplos:

- Aumento significativo de errores.
- Caída en generación de rutas.
- Fallos de pagos.
- Problemas con proveedores externos.
- Incremento anormal del tiempo de respuesta.

Las alertas deberán concentrarse en problemas que requieran acción.


---

23. Control de calidad de eventos

Antes del lanzamiento deberán probarse los eventos.

Se deberá comprobar:

- Que se activan en el momento correcto.
- Que no se duplican.
- Que los nombres son consistentes.
- Que las propiedades son correctas.
- Que no contienen datos innecesarios.
- Que los embudos pueden reconstruirse.

Una analítica mal implementada puede producir decisiones incorrectas.


---

24. Documentación de eventos

ZAREVOA deberá mantener un registro técnico de eventos.

Para cada evento se podrá documentar:

Nombre.

Descripción.

Momento de activación.

Propiedades.

Finalidad.

Plataforma o pantalla.

Estado de implementación.

Esto permitirá mantener consistencia a medida que el producto crezca.


---

25. Privacidad y consentimiento

La implementación deberá cumplir las obligaciones aplicables en los mercados donde opere ZAREVOA.

Cuando corresponda deberán existir mecanismos para:

- Informar al usuario.
- Solicitar consentimiento.
- Gestionar preferencias.
- Rechazar tecnologías no esenciales.
- Eliminar o gestionar información según corresponda.

La privacidad deberá formar parte de la arquitectura desde el inicio.


---

26. Revisión periódica

Los eventos deberán revisarse periódicamente.

Se eliminarán aquellos que:

- Ya no se utilizan.
- Generan datos redundantes.
- No ayudan a tomar decisiones.
- Recopilan información innecesaria.

También podrán añadirse nuevos eventos cuando aparezcan preguntas importantes que los datos actuales no permitan responder.


---

27. Principio final

La analítica de ZAREVOA deberá servir para comprender al producto, no para vigilar al viajero.

La regla será:

Medir lo necesario.

Proteger lo personal.

Comprender el comportamiento.

Detectar problemas.

Aprender.

Mejorar.

Los datos tendrán valor únicamente cuando permitan construir una experiencia de viaje mejor.
