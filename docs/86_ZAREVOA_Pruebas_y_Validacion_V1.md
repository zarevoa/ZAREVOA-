ZAREVOA — Pruebas y Validación V1

Documento 86


1. Objetivo

Este documento define la estrategia de pruebas y validación de ZAREVOA V1 antes de su lanzamiento público.

El objetivo será comprobar que la plataforma funciona técnicamente, que las recomendaciones tienen sentido y que una persona puede completar una planificación sin dificultades importantes.

ZAREVOA no deberá considerarse listo únicamente porque el sistema funcione.

También deberá demostrar que resulta útil para viajeros reales.


---

2. Principio de validación

La validación de ZAREVOA deberá considerar tres dimensiones:

Funciona.

Se entiende.

Es útil.

Una función técnicamente correcta puede necesitar cambios si los usuarios no comprenden cómo utilizarla.

Una interfaz clara puede necesitar cambios si las recomendaciones obtenidas no aportan suficiente valor.

Las tres dimensiones deberán evaluarse conjuntamente.


---

3. Etapas de prueba

Las pruebas podrán dividirse en:

Etapa 1:
Pruebas internas.

Etapa 2:
Pruebas funcionales.

Etapa 3:
Pruebas del ZAREVOA Engine.

Etapa 4:
Pruebas de experiencia de usuario.

Etapa 5:
Usuarios reales controlados.

Etapa 6:
Lanzamiento limitado.

Etapa 7:
Validación posterior al lanzamiento.


---

4. Pruebas internas

Antes de invitar usuarios externos se comprobarán los flujos principales.

Entre ellos:

- Inicio de planificación.
- Travel Profile.
- Generación de ruta.
- Modificación de ruta.
- Generación de itinerario.
- Guardado.
- Recuperación de viajes.
- Registro e inicio de sesión cuando corresponda.
- Opciones comerciales cuando estén activas.
- Funcionamiento móvil.

Los errores evidentes deberán corregirse antes de ampliar las pruebas.


---

5. Pruebas del Travel Profile

Se deberá comprobar que las preguntas:

- Son comprensibles.
- Tienen una finalidad clara.
- No son innecesariamente numerosas.
- Funcionan correctamente en móvil.
- Permiten volver atrás.
- Conservan las respuestas.
- Admiten diferentes tipos de viajeros.

También deberá comprobarse que las respuestas afectan realmente a la planificación cuando corresponde.


---

6. Pruebas del ZAREVOA Engine

El motor deberá probarse utilizando perfiles de viaje muy diferentes.

Por ejemplo:

- Viajero solo.
- Pareja.
- Familia.
- Grupo de amigos.
- Viaje corto.
- Viaje largo.
- Presupuesto limitado.
- Presupuesto alto.
- Ritmo relajado.
- Ritmo equilibrado.
- Ritmo intenso.
- Intereses muy específicos.
- Primer viaje a un destino.
- Viajero que ya conoce parte del destino.

El objetivo será comprobar que el sistema no produce prácticamente la misma ruta para todos.


---

7. Pruebas de duración

Se deberán probar viajes con distintas cantidades de días.

Ejemplos:

3 días.

5 días.

7 días.

10 días.

14 días.

21 días.

30 días.

El motor deberá evitar añadir destinos simplemente porque existen más días y deberá mantener una distribución lógica.


---

8. Pruebas de traslados

Se comprobará que ZAREVOA considere el tiempo real asociado a los cambios de destino.

Esto incluye:

- Salida del alojamiento.
- Traslado hacia estación o aeropuerto.
- Espera.
- Trayecto.
- Llegada.
- Traslado al nuevo alojamiento.
- Check-in.
- Tiempo razonable de adaptación.

Los días de transición deberán tener una carga de actividades menor cuando corresponda.


---

9. Pruebas de vuelos

Se probarán especialmente:

- Día de llegada.
- Día de salida.
- Vuelos nocturnos.
- Llegadas tempranas.
- Llegadas tardías.
- Escalas.
- Cambios importantes de zona horaria.

ZAREVOA deberá evitar generar itinerarios poco realistas inmediatamente después de viajes largos.


---

10. Pruebas de ritmo

El mismo viaje deberá probarse con diferentes ritmos.

Relajado:
Menos actividades y mayor margen.

Equilibrado:
Balance entre actividades y tiempo libre.

Intenso:
Mayor cantidad de actividades sin crear una planificación físicamente irreal.

La diferencia deberá ser visible para el usuario.


---

11. Pruebas de presupuesto

Se deberán comprobar los niveles:

Económico.

Equilibrado.

Confort.

Premium.

También deberán probarse presupuestos definidos por el usuario.

El sistema deberá adaptar decisiones cuando sea posible sin asumir que un presupuesto mayor obliga a utilizar opciones más costosas.


---

12. Pruebas de intereses

Se crearán perfiles con intereses diferentes.

Ejemplos:

Historia.

Gastronomía.

Naturaleza.

Arquitectura.

Fotografía.

Playas.

Aventura.

Compras.

Vida nocturna.

Cultura.

La selección de actividades y el peso de los destinos deberán cambiar de forma razonable según estos intereses.


---

13. Must See y For You

Las pruebas deberán comprobar la diferencia entre:

Must See:
Experiencias especialmente relevantes o emblemáticas dentro del viaje.

For You:
Experiencias seleccionadas por su relación específica con el Travel Profile.

No todo lugar popular deberá convertirse automáticamente en Must See.

No toda recomendación personalizada deberá desplazar una experiencia esencial.


---

14. Composición del grupo

Se probarán diferentes composiciones de viajeros.

El sistema deberá considerar edades y características relevantes sin utilizar estereotipos.

Por ejemplo, no deberá asumir automáticamente que:

Una persona mayor quiere pocas actividades.

Una familia solamente quiere actividades infantiles.

Una persona joven quiere vida nocturna.

Las preferencias expresadas deberán tener mayor peso que las suposiciones.


---

15. Modificación de ruta

Una prueba fundamental será modificar una ruta ya generada.

Se comprobará que el usuario pueda:

- Añadir un destino.
- Eliminar un destino.
- Cambiar días.
- Cambiar ritmo.
- Ajustar presupuesto.
- Modificar intereses cuando corresponda.

ZAREVOA deberá recalcular sin obligar a completar nuevamente todo el Travel Profile.


---

16. Casos extremos

También deberán probarse situaciones poco habituales.

Ejemplos:

- Muy pocos días para demasiados destinos.
- Presupuesto incompatible con las preferencias.
- Grupo numeroso.
- Destinos muy alejados entre sí.
- Fechas con disponibilidad limitada.
- Información incompleta.
- Preferencias contradictorias.

ZAREVOA deberá responder de forma útil y explicar las limitaciones en lugar de generar silenciosamente una planificación deficiente.


---

17. Datos reales

Cuando ZAREVOA utilice datos externos se comprobará:

- Exactitud.
- Actualización.
- Fuente.
- Disponibilidad.
- Manejo de errores.
- Respuesta cuando un proveedor no esté disponible.

El sistema deberá evitar presentar información incierta como un hecho confirmado.


---

18. Pruebas de dispositivos

Como mínimo deberán probarse:

- Teléfonos Android.
- iPhone.
- Computadores de escritorio.
- Diferentes tamaños de pantalla.

También deberán revisarse los principales navegadores compatibles.

La experiencia móvil tendrá especial importancia.


---

19. Rendimiento

Se comprobarán:

- Tiempo de carga.
- Tiempo de generación de ruta.
- Tiempo de generación de itinerario.
- Respuesta al modificar.
- Guardado.
- Recuperación de información.

Cuando una operación requiera espera, el usuario deberá recibir una señal clara de que el sistema continúa funcionando.


---

20. Errores y recuperación

Se simularán fallos como:

- Pérdida temporal de conexión.
- Error de API.
- Error durante generación.
- Pago rechazado cuando corresponda.
- Sesión interrumpida.
- Recarga accidental de página.

Siempre que sea posible, el trabajo realizado por el usuario deberá conservarse.


---

21. Pruebas de privacidad y seguridad

Antes del lanzamiento deberán comprobarse aspectos relacionados con:

- Acceso a cuentas.
- Autorización.
- Protección de datos.
- Sesiones.
- Recuperación de contraseña.
- Exposición accidental de información.
- Formularios.
- Integraciones externas.

Los problemas de seguridad importantes deberán bloquear el lanzamiento hasta ser corregidos.


---

22. Usuarios de prueba

Después de las pruebas internas se invitará a un grupo reducido de personas.

Será conveniente incluir diferentes perfiles de viajeros.

No deberán recibir instrucciones excesivamente detalladas.

El objetivo será observar si pueden comprender ZAREVOA por sí mismos.


---

23. Observación

Durante las pruebas se observará:

- Dónde dudan.
- Qué preguntas no comprenden.
- Qué botones no encuentran.
- Qué información esperan ver.
- Qué modifican.
- Qué les sorprende.
- Qué consideran innecesario.
- En qué momento abandonan.

Lo que el usuario hace puede ser más informativo que lo que dice.


---

24. Preguntas posteriores

Después de completar una prueba podrán utilizarse preguntas breves.

Ejemplos:

“¿Entendiste cómo funciona ZAREVOA?”

“¿La ruta tiene sentido para ti?”

“¿Qué cambiarías?”

“¿Hubo algún momento confuso?”

“¿Utilizarías este itinerario en un viaje real?”

“¿Volverías a utilizar ZAREVOA?”

Las respuestas deberán registrarse de manera estructurada.


---

25. Clasificación de problemas

Los problemas detectados podrán clasificarse como:

Crítico:
Impide utilizar ZAREVOA o representa un riesgo importante.

Alto:
Afecta seriamente la experiencia o calidad de la planificación.

Medio:
Genera dificultad pero existe una alternativa.

Bajo:
Mejora deseable que no impide utilizar el producto.

Esta clasificación permitirá priorizar el trabajo antes del lanzamiento.


---

26. Criterios mínimos para lanzamiento

Antes de abrir ZAREVOA públicamente deberá comprobarse como mínimo que:

- El flujo principal funciona.
- El Travel Profile puede completarse.
- La ruta puede generarse.
- Las recomendaciones son razonablemente coherentes.
- La ruta puede modificarse.
- El itinerario puede generarse.
- La experiencia móvil funciona correctamente.
- Los datos se guardan de manera adecuada.
- No existen errores críticos conocidos.
- Las principales medidas de privacidad y seguridad están implementadas.
- Usuarios de prueba consiguen utilizar el producto sin asistencia constante.


---

27. Lanzamiento limitado

Antes de realizar campañas importantes podrá utilizarse un lanzamiento limitado.

Esto permitirá observar:

- Usuarios reales.
- Comportamiento no previsto.
- Costos tecnológicos.
- Errores.
- Conversión.
- Calidad de recomendaciones.
- Solicitudes de soporte.

La adquisición podrá aumentarse gradualmente a medida que la plataforma demuestre estabilidad.


---

28. Validación continua

El lanzamiento no finalizará el proceso de pruebas.

Los datos reales deberán utilizarse para continuar evaluando:

- Nuevos destinos.
- Nuevos perfiles.
- Cambios del Engine.
- Nuevas funciones.
- Integraciones.
- Productos comerciales.

Cada cambio importante deberá probarse antes de llegar a todos los usuarios.


---

29. Registro de pruebas

ZAREVOA deberá mantener un registro sencillo que permita conocer:

- Qué se probó.
- Cuándo.
- Resultado.
- Problemas encontrados.
- Prioridad.
- Responsable cuando corresponda.
- Estado de corrección.
- Nueva validación.

Esto evitará perder problemas o repetir pruebas innecesariamente.


---

30. Principio final

ZAREVOA V1 no necesita ser perfecto para lanzarse.

Sí necesita ser:

Funcional.

Comprensible.

Confiable.

Útil.

Seguro.

Y suficientemente bueno para que viajeros reales quieran utilizarlo.

La validación no buscará demostrar que ZAREVOA no tiene errores.

Buscará comprobar que ZAREVOA resuelve correctamente un problema real y que existe una base sólida sobre la cual seguir mejorando.
