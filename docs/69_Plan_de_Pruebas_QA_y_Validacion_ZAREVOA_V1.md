DOCUMENTO 69 — PLAN DE PRUEBAS, QA Y VALIDACIÓN ZAREVOA V1

1. Objetivo

Definir cómo deberá probarse ZAREVOA V1 antes de su lanzamiento público para comprobar que la plataforma funciona correctamente, genera rutas coherentes y ofrece una experiencia suficientemente confiable para usuarios reales.

El objetivo no será demostrar que ZAREVOA es perfecto.

Será detectar y corregir los problemas importantes antes de comenzar a crecer.

2. Principio fundamental

Una función no estará terminada únicamente porque técnicamente funcione.

También deberá comprobarse que:

- el usuario la entiende;
- produce el resultado esperado;
- funciona en diferentes dispositivos;
- maneja correctamente los errores;
- no genera recomendaciones absurdas;
- mantiene una experiencia coherente.

El principio será:

Construir → Probar → Detectar → Corregir → Volver a probar.

3. Áreas principales de prueba

ZAREVOA V1 deberá probarse al menos en:

- registro y acceso;
- Travel Profile;
- generación de ruta;
- modificación de ruta;
- itinerario;
- ZAREVOA Engine;
- datos externos;
- interfaz;
- dispositivos móviles;
- rendimiento;
- seguridad;
- enlaces;
- analítica;
- errores;
- funciones comerciales que estén activas.

4. Registro y cuenta

Se comprobarán situaciones como:

- creación correcta de cuenta;
- correo ya registrado;
- contraseña incorrecta;
- recuperación de contraseña;
- cierre de sesión;
- inicio de sesión posterior;
- eliminación de cuenta cuando esté disponible;
- conservación correcta de información autorizada.

Los mensajes de error deberán ser comprensibles.

5. Travel Profile

Se probará que:

- las preguntas aparezcan correctamente;
- las opciones puedan seleccionarse;
- los datos se guarden;
- el usuario pueda retroceder;
- pueda modificar respuestas;
- los campos obligatorios funcionen;
- las respuestas realmente influyan en el resultado.

También deberá medirse si el formulario resulta demasiado largo o confuso.

6. Pruebas del ZAREVOA Engine

El motor deberá probarse con perfiles muy diferentes.

Ejemplos:

Caso A

10 días en Italia, ritmo relajado, interés cultural y gastronómico.

Caso B

10 días en Italia, ritmo intenso, interés en historia y arquitectura.

Caso C

15 días en Japón, presupuesto económico.

Caso D

7 días en Portugal, familia con niños.

Caso E

20 días por Europa, pareja, presupuesto Premium.

El resultado no debería ser prácticamente idéntico en todos los casos.

La personalización deberá ser visible.

7. Pruebas de duración

Se probarán viajes de diferentes extensiones:

- 2 días;
- 5 días;
- 7 días;
- 10 días;
- 15 días;
- 30 días o más.

ZAREVOA deberá evitar introducir demasiados destinos cuando el tiempo disponible sea reducido.

8. Pruebas de ritmo

Se comprobará que los modos:

Relajado — Equilibrado — Intenso

produzcan diferencias reales.

Por ejemplo, un viaje relajado deberá:

- reducir cantidad de actividades;
- disminuir cambios innecesarios;
- dejar mayor margen;
- evitar días excesivamente cargados.

9. Traslados

Cada ruta deberá analizar los tiempos reales de transición.

Las pruebas deberán detectar situaciones como:

- actividad programada mientras el usuario está viajando;
- traslado entre ciudades imposible;
- conexión demasiado ajustada;
- exceso de actividades después de un vuelo;
- cambio de alojamiento sin beneficio suficiente.

Los días de traslado deberán tener una carga razonable.

10. Bases

Se comprobará que ZAREVOA utilice correctamente el concepto de base.

Ejemplo:

Si varias actividades pueden realizarse desde una misma ciudad, el sistema deberá evitar recomendar cambios de alojamiento innecesarios.

La cantidad de bases deberá tener relación con:

- duración;
- distancias;
- ritmo;
- objetivos del viaje.

11. Presupuesto

Se probarán los niveles:

- Económico;
- Equilibrado;
- Confort;
- Premium.

También deberán probarse presupuestos definidos por el usuario.

El sistema deberá adaptar las decisiones y no limitarse a cambiar etiquetas.

12. Intereses

Se comprobará que los intereses realmente modifiquen las recomendaciones.

Se distinguirá entre:

Must See

y

For You.

Un lugar famoso podrá aparecer como importante, pero ZAREVOA deberá priorizar también aquello que tenga mayor relación con el perfil específico del viajero.

13. Composición del grupo

Se probarán diferentes configuraciones:

- persona sola;
- pareja;
- amigos;
- familia;
- grupos con diferentes edades.

Las recomendaciones deberán adaptarse sin utilizar estereotipos automáticos.

Las preferencias declaradas tendrán mayor importancia que asumir intereses únicamente por edad.

14. Modificación de ruta

Una prueba crítica será modificar una ruta ya generada.

Ejemplos:

- eliminar una ciudad;
- añadir un destino;
- cambiar noches;
- modificar presupuesto;
- cambiar ritmo;
- sustituir una actividad.

ZAREVOA deberá recalcular la parte necesaria sin obligar al usuario a comenzar nuevamente todo el formulario.

15. “Tu ruta recomendada”

Antes del itinerario detallado deberá probarse la pantalla:

Tu ruta recomendada

El usuario deberá poder comprender fácilmente:

- destinos;
- orden;
- noches;
- bases;
- lógica general.

Desde allí deberá poder:

Aprobar o Modificar.

Esta pantalla será una validación fundamental antes de que el Engine realice trabajo adicional.

16. Pruebas de información externa

Cuando ZAREVOA dependa de información externa deberán probarse situaciones como:

- API disponible;
- API lenta;
- información incompleta;
- proveedor sin resultados;
- error de conexión;
- precio no disponible;
- servicio temporalmente caído.

La plataforma deberá degradarse de forma controlada en lugar de romper completamente la experiencia.

17. Pruebas de interfaz

Se revisará cada pantalla comprobando:

- textos;
- botones;
- navegación;
- espaciado;
- imágenes;
- logotipo;
- tipografía;
- colores;
- coherencia visual;
- estados de carga;
- mensajes de error.

La identidad visual aprobada de ZAREVOA deberá mantenerse de forma consistente.

18. Dispositivos

Como mínimo deberán realizarse pruebas en:

- teléfonos Android;
- iPhone;
- computadores;
- diferentes tamaños de pantalla;
- navegadores principales.

La experiencia móvil tendrá especial prioridad.

19. Rendimiento

Se medirán:

- tiempo de carga;
- tiempo de generación;
- respuesta del Engine;
- peso de páginas;
- consumo de recursos;
- errores bajo carga.

Cuando una generación requiera varios segundos, el usuario deberá recibir información visual de que ZAREVOA continúa trabajando.

20. Seguridad

Antes del lanzamiento deberán comprobarse aspectos básicos como:

- autenticación;
- permisos;
- protección de rutas privadas;
- exposición de claves;
- configuración de APIs;
- validación de entradas;
- accesos no autorizados;
- dependencias vulnerables.

Las claves privadas nunca deberán quedar expuestas en repositorios públicos o código enviado al navegador.

21. Analítica

Se verificará que los eventos importantes realmente estén registrándose.

Ejemplos:

- inicio de planificación;
- Travel Profile completado;
- ruta generada;
- ruta modificada;
- itinerario creado;
- enlace compartido;
- clic comercial;
- compra cuando corresponda.

Una analítica incorrecta puede producir decisiones equivocadas.

22. Pruebas con usuarios reales

Antes del lanzamiento abierto deberá existir una etapa con usuarios externos al desarrollo.

Idealmente deberán participar personas con diferentes:

- edades;
- experiencia viajando;
- conocimientos tecnológicos;
- presupuestos;
- tipos de viaje.

No se les deberá explicar cada pantalla previamente.

El objetivo será observar si pueden utilizar ZAREVOA por sí mismos.

23. Registro de problemas

Cada problema detectado deberá registrarse con:

- descripción;
- pantalla;
- pasos para reproducir;
- resultado esperado;
- resultado obtenido;
- gravedad;
- estado.

Los errores deberán clasificarse.

Crítico

Impide utilizar una función principal o compromete seguridad/datos.

Alto

Produce resultados incorrectos importantes.

Medio

Afecta la experiencia, pero existe alternativa.

Bajo

Problema visual o menor que no bloquea el uso.

24. Criterios mínimos para lanzamiento

ZAREVOA V1 podrá considerarse preparado para lanzamiento controlado cuando:

- no existan errores críticos conocidos;
- registro y acceso funcionen;
- Travel Profile funcione;
- Engine genere rutas coherentes;
- “Tu ruta recomendada” funcione;
- las rutas puedan modificarse;
- el itinerario pueda generarse;
- la experiencia móvil sea utilizable;
- la analítica básica funcione;
- privacidad y documentos legales mínimos estén disponibles;
- exista un mecanismo para reportar problemas.

25. Beta controlada

Antes del lanzamiento general podrá utilizarse una beta limitada.

Ejemplo:

20–50 usuarios iniciales.

Después:

100–500 usuarios.

El número exacto dependerá de:

- estabilidad;
- costos;
- capacidad de soporte;
- resultados.

El objetivo será aprender antes de invertir fuertemente en adquisición.

26. Decisión de lanzamiento

La decisión final no deberá basarse únicamente en:

“Ya terminamos de programar.”

Deberá responder:

¿Una persona que nunca ha visto ZAREVOA puede entrar, entenderlo, crear un viaje y obtener una ruta que considere útil?

Si la respuesta es consistentemente positiva, ZAREVOA estará preparado para comenzar su siguiente etapa.

27. Principio final

La primera versión pública de ZAREVOA no necesitará contener todas las funciones imaginadas para el futuro.

Necesitará hacer muy bien su función esencial:

comprender al viajero y convertir sus preferencias en una ruta coherente, personalizada y fácil de utilizar.

Todo lo demás podrá evolucionar a partir de usuarios y viajes reales.

---

Estado: Plan de pruebas, QA y validación definido para ZAREVOA V1.

Aplicación: Desarrollo, ZAREVOA Engine, interfaz, beta, seguridad y preparación para lanzamiento.
