ZAREVOA — Technical Architecture V1

1. Objetivo

Este documento define la arquitectura técnica inicial de ZAREVOA V1.

La arquitectura debe permitir construir un producto sólido, escalable y fácil de evolucionar, sin añadir complejidad innecesaria durante la primera versión.

ZAREVOA V1 será inicialmente una aplicación web responsive, accesible desde computador, tablet y teléfono móvil.

La arquitectura estará diseñada para que futuras versiones puedan incorporar nuevas funciones, integraciones y productos sin tener que reconstruir el sistema desde cero.

---

2. Principio de arquitectura

ZAREVOA no dependerá exclusivamente de inteligencia artificial.

El sistema combinará tres componentes principales:

Datos reales + Reglas propias ZAREVOA + Inteligencia Artificial

Cada componente tendrá una función diferente.

Datos reales

Entregan información verificable sobre:

- destinos;
- distancias;
- tiempos de traslado;
- transporte;
- alojamientos;
- actividades;
- horarios;
- precios cuando estén disponibles;
- ubicación geográfica;
- información práctica del viaje.

Reglas ZAREVOA

Representan el criterio propio del producto.

Permiten decidir:

- cuántas bases utilizar;
- cuánto tiempo permanecer en cada lugar;
- cuándo un traslado consume una parte importante del día;
- cuántas actividades son razonables;
- cómo adaptar el viaje al ritmo elegido;
- cómo distribuir el presupuesto;
- cómo priorizar intereses;
- cuándo una actividad realmente tiene sentido dentro de la ruta.

Inteligencia Artificial

La IA funcionará como una capa interna de planificación y razonamiento.

Su función será interpretar el Travel Profile, combinar información, generar propuestas, explicar decisiones y personalizar el resultado.

La IA no sustituirá las reglas estructurales de ZAREVOA.

---

3. Flujo principal del sistema

El flujo general de ZAREVOA V1 será:

Usuario → Travel Profile → ZAREVOA Engine → Tu ruta recomendada → Aprobación o modificación → Itinerario detallado → Journey

El sistema no generará inmediatamente un itinerario completo.

Primero deberá construir una ruta lógica.

El usuario verá:

Tu ruta recomendada

Esta etapa mostrará las bases principales del viaje, noches aproximadas, traslados y lógica general de la propuesta.

El usuario podrá:

- aprobar la ruta;
- modificarla;
- cambiar destinos;
- ajustar prioridades;
- solicitar una nueva propuesta.

Solo después de esta etapa se generará el itinerario detallado.

---

4. Travel Profile

El Travel Profile será la estructura central de entrada de información.

Podrá contener:

- destino o región;
- fechas;
- duración;
- número de viajeros;
- composición del grupo;
- edades cuando sean relevantes;
- presupuesto;
- nivel de presupuesto;
- intereses;
- prioridades;
- lugares Must See;
- ritmo de viaje;
- preferencias;
- restricciones;
- necesidades especiales;
- información adicional aportada por el usuario.

El Travel Profile deberá permanecer editable durante el proceso.

Modificar una variable no deberá obligar al usuario a comenzar nuevamente todo el formulario.

---

5. ZAREVOA Engine V1

El ZAREVOA Engine V1 será el núcleo de planificación.

Su arquitectura conceptual será modular.

5.1 Validator

Revisa que la información necesaria exista y detecta inconsistencias.

Ejemplos:

- fechas incompatibles;
- duración incorrecta;
- presupuesto insuficientemente definido;
- destinos imposibles dentro del tiempo disponible;
- información crítica faltante.

5.2 Route Builder

Construye posibles estructuras de viaje.

Determina:

- bases;
- número de noches;
- orden geográfico;
- desplazamientos;
- días de transición;
- coherencia general de la ruta.

5.3 ZAREVOA Scoring

Evalúa cada alternativa utilizando criterios propios.

Principio general:

Interés + tiempo + logística + presupuesto + ritmo + coherencia de ruta

Una alternativa con más lugares no necesariamente tendrá una mejor puntuación.

ZAREVOA deberá favorecer viajes realizables y coherentes.

5.4 AI Planner

Utiliza inteligencia artificial para:

- interpretar preferencias;
- conectar intereses;
- personalizar propuestas;
- generar explicaciones;
- ayudar a construir el itinerario;
- adaptar recomendaciones al contexto del viajero.

5.5 Verifier

Comprueba la coherencia del resultado antes de presentarlo.

Debe detectar:

- tiempos imposibles;
- exceso de actividades;
- traslados mal calculados;
- contradicciones;
- recomendaciones fuera de contexto;
- información que requiera verificación adicional.

5.6 Presenter

Transforma el resultado técnico del Engine en información clara y comprensible para el usuario.

---

6. Salida estructurada del Engine

El Engine deberá producir información estructurada antes de generar texto para el usuario.

Ejemplo conceptual:

- ruta;
- bases;
- noches;
- motivos de cada base;
- traslados;
- tiempos de transición;
- días afectados por desplazamientos;
- actividades prioritarias;
- presupuesto estimado;
- advertencias;
- recomendaciones;
- nivel de confianza de la información.

Esto permitirá que diferentes interfaces utilicen el mismo resultado sin depender directamente del texto generado por IA.

---

7. Niveles de información

Cuando sea necesario, ZAREVOA podrá distinguir información según su origen o nivel de certeza.

VERIFIED

Información obtenida de una fuente verificable o servicio confiable.

ZAREVOA

Decisión o recomendación generada mediante reglas propias del sistema.

ESTIMATED

Estimación razonable utilizada para planificación.

UNKNOWN

Información que todavía no puede confirmarse.

El sistema deberá evitar presentar una estimación como si fuera un hecho confirmado.

---

8. Duración y número de bases

El Engine deberá evitar viajes fragmentados innecesariamente.

Como referencia inicial:

- 1–3 días: normalmente 1 base;
- 4–6 días: normalmente 1–2 bases;
- 7–10 días: normalmente 2–3 bases;
- viajes más largos podrán incorporar bases adicionales cuando exista una razón logística o experiencial.

Estas reglas serán orientativas y podrán adaptarse según:

- geografía;
- distancias;
- transporte;
- intereses;
- presupuesto;
- ritmo;
- contexto real del viaje.

---

9. Ritmo de viaje

ZAREVOA V1 manejará tres niveles:

Relajado

Menos actividades, más tiempo libre y mayor margen entre desplazamientos.

Equilibrado

Balance entre actividades, descanso y exploración.

Intenso

Mayor cantidad de actividades, siempre que sean logísticamente razonables.

El ritmo deberá afectar realmente la planificación y no funcionar únicamente como una etiqueta visual.

---

10. Tiempo real de transición

ZAREVOA deberá considerar el tiempo real necesario para cambiar de ubicación.

Un traslado no será únicamente el tiempo indicado por un avión, tren o vehículo.

Podrá incluir:

alojamiento → terminal/aeropuerto → espera → transporte → llegada → desplazamiento → nuevo alojamiento

Cuando un traslado consuma una parte importante del día, el Engine deberá reducir automáticamente la cantidad de actividades previstas.

---

11. Presupuesto

ZAREVOA V1 manejará niveles iniciales:

- Económico;
- Equilibrado;
- Confort;
- Premium.

También permitirá introducir un presupuesto definido por el usuario.

El presupuesto podrá distribuirse entre:

- alojamiento;
- transporte;
- alimentación;
- actividades;
- experiencias;
- margen adicional.

La distribución deberá ser adaptable.

No todos los viajeros valoran las mismas categorías de gasto.

---

12. Intereses y prioridades

El Engine distinguirá principalmente entre:

Must See

Lugares o experiencias que el viajero considera prioritarios.

For You

Recomendaciones personalizadas por ZAREVOA basadas en el Travel Profile.

Antes de recomendar una actividad, el sistema deberá evaluar:

1. interés del viajero;
2. tiempo real disponible;
3. ubicación;
4. logística;
5. presupuesto;
6. ritmo;
7. sentido dentro de la ruta.

Una actividad popular no deberá recomendarse automáticamente si no aporta valor al viaje específico.

---

13. Composición del grupo

ZAREVOA podrá considerar:

- viajeros individuales;
- parejas;
- familias;
- grupos;
- niños;
- adultos;
- adultos mayores.

La edad o composición del grupo servirá como contexto, no como estereotipo.

Las preferencias expresadas por los viajeros tendrán prioridad sobre supuestos automáticos basados únicamente en edad.

---

14. Recomendaciones y reservas

La arquitectura deberá separar claramente:

Recomendación genuina

Una opción recomendada porque ZAREVOA considera que es adecuada para el viajero.

Opción reservable

Una opción que además permite acceder a un proveedor externo para realizar una reserva.

Opción comisionable

Una reserva que puede generar ingresos de afiliación o comisión para ZAREVOA.

La existencia de una comisión no deberá determinar por sí sola qué opción se recomienda.

El criterio del viajero debe mantenerse como prioridad.

---

15. Modificación de rutas

Una característica importante de ZAREVOA será la capacidad de modificar una ruta sin reiniciar todo el proceso.

Ejemplos:

- cambiar una ciudad;
- añadir una noche;
- eliminar una base;
- reducir actividades;
- cambiar presupuesto;
- modificar ritmo;
- añadir un Must See.

El Engine deberá recalcular únicamente las partes afectadas cuando sea técnicamente posible.

---

16. Arquitectura de datos

Para V1 se utilizará una arquitectura de datos sencilla pero preparada para crecer.

Conceptualmente podrá utilizarse una base de datos relacional como PostgreSQL, mediante una plataforma como Supabase u otra solución equivalente.

La base de datos podrá almacenar:

- perfiles de viaje;
- preferencias;
- rutas;
- itinerarios;
- destinos;
- actividades;
- reglas;
- productos ZAREVOA;
- estados del Journey;
- información operativa necesaria.

La implementación definitiva se decidirá durante el desarrollo técnico.

---

17. Servicios externos

ZAREVOA podrá conectarse progresivamente con servicios externos para obtener información útil.

Ejemplos:

- mapas;
- geolocalización;
- transporte;
- clima;
- actividades;
- alojamientos;
- vuelos;
- proveedores de reservas;
- sistemas de afiliación.

Las integraciones se incorporarán gradualmente según su importancia para V1.

El producto no deberá depender desde el primer día de una gran cantidad de APIs costosas.

---

18. Frontend

La primera versión será una aplicación web responsive.

La interfaz deberá priorizar:

- simplicidad;
- claridad;
- velocidad;
- navegación móvil;
- consistencia visual;
- facilidad para modificar decisiones;
- presentación clara de rutas e itinerarios.

Las pantallas deberán consumir información estructurada del sistema y no depender directamente de respuestas libres de IA.

---

19. Backend

El backend será responsable de:

- recibir el Travel Profile;
- validar información;
- ejecutar reglas;
- consultar datos;
- comunicarse con servicios externos;
- interactuar con modelos de IA;
- almacenar viajes;
- generar rutas;
- recalcular cambios;
- controlar estados;
- entregar resultados estructurados al frontend.

La lógica crítica de ZAREVOA deberá permanecer en el backend y no depender únicamente del dispositivo del usuario.

---

20. Seguridad y privacidad

ZAREVOA deberá aplicar desde V1 principios básicos de seguridad.

Entre ellos:

- recopilar únicamente información necesaria;
- evitar almacenar datos sensibles sin una razón funcional;
- proteger credenciales y claves de servicios externos;
- utilizar conexiones seguras;
- controlar acceso a información privada;
- separar datos públicos de datos personales;
- permitir evolución futura de las políticas de privacidad.

---

21. Escalabilidad

La arquitectura deberá permitir incorporar posteriormente:

- nuevas fuentes de datos;
- más destinos;
- nuevos motores de recomendación;
- mejores modelos de IA;
- reservas;
- afiliados;
- pagos;
- cuentas de usuario más avanzadas;
- colaboración entre viajeros;
- nuevas funciones Journey;
- productos ZAREVOA adicionales.

La prioridad de V1 será validar el producto antes de construir infraestructura innecesariamente compleja.

---

22. Fuera del alcance inicial de V1

No será prioridad inicial:

- aplicaciones nativas independientes para Android e iOS;
- sistema propio completo de reservas;
- infraestructura propia de pagos internacionales;
- almacenamiento de información altamente sensible;
- integraciones con todos los proveedores turísticos existentes;
- automatizaciones complejas que todavía no hayan demostrado valor para el usuario.

Estas capacidades podrán evaluarse después de validar ZAREVOA V1.

---

23. Principio técnico final

La tecnología deberá estar al servicio del criterio de viaje.

ZAREVOA no buscará generar simplemente más recomendaciones.

Buscará generar mejores decisiones de viaje.

La arquitectura debe permitir que datos reales, reglas propias e inteligencia artificial trabajen conjuntamente para crear viajes:

coherentes, personalizados, realizables, transparentes y humanos.

---

Documento: 07 — ZAREVOA Technical Architecture
Proyecto: ZAREVOA
Versión: V1
Estado: Arquitectura técnica inicial aprobada
