133 — PLAN DE PRUEBAS ZAREVOA V1

1. Objetivo

Definir cómo se probará ZAREVOA V1 antes de su lanzamiento para comprobar que el producto funciona correctamente, mantiene el criterio propio de ZAREVOA y entrega una experiencia útil, realista y comprensible para el viajero.

2. Principio general

Las pruebas no deberán limitarse a comprobar que los botones y pantallas funcionen.

ZAREVOA deberá superar dos tipos fundamentales de evaluación:

Prueba técnica: comprobar que el sistema funciona.

Prueba de criterio: comprobar que el viaje propuesto tiene sentido.

Ambas serán necesarias antes del lanzamiento.

3. Etapas de prueba

Las pruebas se realizarán progresivamente:

1. Pruebas por componente.
2. Pruebas de integración.
3. Pruebas del flujo completo.
4. Pruebas del ZAREVOA Engine.
5. Pruebas de datos reales e integraciones.
6. Pruebas de experiencia y usabilidad.
7. Pruebas de seguridad y privacidad.
8. Pruebas con usuarios reales.
9. Prueba final previa al lanzamiento.

4. Pruebas por componente

Cada módulo deberá comprobarse individualmente antes de integrarse con el resto.

Entre ellos:

- Creación de viaje.
- Travel Profile.
- ZAREVOA Engine.
- Tu ruta recomendada.
- Modificación de ruta.
- Itinerario.
- Guardado.
- Recuperación.
- Recomendaciones.
- Cuenta de usuario.
- Pagos, cuando correspondan.

5. Pruebas de integración

Se comprobará que los módulos intercambien correctamente la información.

Por ejemplo:

- Travel Profile → Engine.
- Engine → Ruta recomendada.
- Ruta modificada → nuevo cálculo.
- Ruta aprobada → Itinerario.
- Itinerario → Guardado.
- Recomendaciones → opciones reservables cuando existan.

6. Prueba del flujo completo

Deberá realizarse repetidamente el recorrido:

Inicio → creación del viaje → Travel Profile → análisis → Tu ruta recomendada → modificación o aprobación → itinerario → guardado → salida → recuperación.

La prueba deberá realizarse desde diferentes dispositivos y perfiles.

7. Pruebas del ZAREVOA Engine

Se crearán escenarios controlados para comprobar sus reglas.

Se evaluará especialmente:

- Número de bases.
- Distribución de días.
- Ritmo.
- Tiempo de transición.
- Días de vuelo.
- Días de traslado.
- Presupuesto.
- Intereses.
- Must See.
- For You.
- Composición del grupo.
- Coherencia general.

8. Pruebas comparativas

Se utilizará el mismo destino y duración cambiando solamente determinadas variables.

Ejemplo:

Perfil A: ritmo relajado.

Perfil B: ritmo intenso.

Los resultados deberán presentar diferencias coherentes.

La misma metodología se utilizará para comparar:

- Presupuestos.
- Intereses.
- Must See.
- Composición del grupo.
- Preferencias.

9. Pruebas de rutas

Las rutas generadas deberán revisarse para detectar:

- Exceso de bases.
- Trayectos innecesarios.
- Retrocesos geográficos.
- Distribuciones poco razonables.
- Días desaprovechados.
- Jornadas imposibles.
- Falta de descanso.

10. Pruebas de itinerarios

Cada día deberá analizarse considerando:

- Tiempo disponible.
- Distancias.
- Duración estimada de actividades.
- Traslados.
- Horarios.
- Ritmo.
- Pausas.
- Coherencia geográfica.

Una agenda técnicamente posible pero poco razonable deberá considerarse un problema de calidad.

11. Pruebas de datos reales

Se comprobará que los datos procedentes de servicios externos sean utilizados correctamente.

Especialmente:

- Ubicaciones.
- Distancias.
- Tiempos de trayecto.
- Horarios.
- Disponibilidad.
- Precios cuando estén integrados.

Cuando una fuente no responda, ZAREVOA deberá manejar la situación sin inventar información.

12. Pruebas de modificación

Se comprobarán cambios como:

- Añadir destino.
- Eliminar destino.
- Cambiar número de días.
- Cambiar ritmo.
- Añadir Must See.
- Modificar presupuesto.
- Rechazar una recomendación.

El sistema deberá conservar la información no afectada y recalcular lo necesario.

13. Pruebas de guardado y recuperación

Se verificará que el usuario pueda:

1. Crear un viaje.
2. Guardarlo.
3. Cerrar sesión o abandonar la plataforma.
4. Regresar.
5. Recuperarlo correctamente.
6. Continuar editándolo.

14. Pruebas de errores

Se provocarán situaciones controladas como:

- Pérdida de conexión.
- API no disponible.
- Datos incompletos.
- Respuesta inválida.
- Tiempo de espera excesivo.
- Error durante generación.

El sistema deberá responder de forma comprensible y evitar pérdida innecesaria de información.

15. Pruebas responsive

Se comprobará el funcionamiento en:

- Teléfonos pequeños.
- Teléfonos grandes.
- Tablets.
- Computadores portátiles.
- Pantallas de escritorio.

La prioridad será que el flujo principal resulte cómodo desde un smartphone.

16. Pruebas de navegadores

Antes del lanzamiento deberán comprobarse los navegadores más relevantes para los usuarios objetivo.

Como mínimo se evaluarán versiones actuales de los principales navegadores utilizados en móvil y escritorio.

17. Pruebas de rendimiento

Se medirán:

- Carga inicial.
- Navegación.
- Generación de rutas.
- Generación de itinerarios.
- Guardado.
- Recuperación.

Cuando exista una espera inevitable deberá mostrarse claramente el estado del proceso.

18. Pruebas de seguridad

Antes de recibir usuarios reales se comprobará, como mínimo:

- Autenticación.
- Autorización.
- Protección de sesiones.
- Gestión de credenciales.
- Acceso a viajes de otros usuarios.
- Exposición accidental de datos.
- Configuración de servicios externos.

19. Pruebas de privacidad

Se verificará que:

- Se recopilen únicamente datos necesarios.
- Las políticas correspondan al funcionamiento real.
- El usuario reciba información adecuada.
- Los datos no se expongan innecesariamente.

20. Pruebas de monetización

Cuando existan productos pagados, afiliados o reservas se comprobará:

- Flujo de pago.
- Confirmación.
- Errores.
- Registro.
- Enlaces.
- Identificación adecuada de opciones externas.

La monetización no deberá alterar negativamente el criterio de recomendación.

21. Usuarios de prueba

Antes de un lanzamiento amplio se seleccionará un grupo pequeño de personas con perfiles diferentes.

Será conveniente incluir:

- Personas con distinta experiencia viajando.
- Diferentes edades.
- Viajeros solos.
- Parejas.
- Familias o grupos.
- Personas con diferentes presupuestos e intereses.

22. Qué observar en usuarios reales

Además de preguntar opiniones, se deberá observar:

- Dónde dudan.
- Qué preguntas no entienden.
- Qué intentan pulsar.
- Qué información esperan encontrar.
- Qué partes modifican.
- En qué momento abandonan.
- Si comprenden por qué ZAREVOA recomienda una ruta.

23. Registro de incidencias

Cada problema relevante deberá registrarse indicando:

- Descripción.
- Pasos para reproducirlo.
- Resultado esperado.
- Resultado obtenido.
- Gravedad.
- Estado de corrección.

24. Clasificación de errores

Los errores podrán clasificarse como:

Crítico: impide utilizar una función esencial, compromete datos o genera un riesgo importante.

Alto: afecta significativamente la experiencia o produce resultados incorrectos.

Medio: genera dificultades pero existe una alternativa razonable.

Bajo: problema menor de presentación, texto o comodidad.

25. Criterio previo al lanzamiento

No deberán existir errores críticos conocidos.

Los errores altos deberán resolverse o contar con una justificación excepcional y un plan inmediato de corrección.

Los problemas menores podrán priorizarse posteriormente cuando no afecten la experiencia esencial.

26. Regresión

Cada vez que se realice una modificación importante deberá comprobarse que funciones anteriormente correctas no hayan dejado de funcionar.

Las pruebas repetitivas deberán automatizarse progresivamente cuando resulte conveniente.

27. Prueba final

Antes del lanzamiento se realizará una simulación completa como si se tratara de un usuario real que nunca ha utilizado ZAREVOA.

No deberán utilizarse conocimientos internos para superar pasos confusos.

La plataforma deberá poder explicarse por sí misma.

28. Resultado esperado

El plan de pruebas deberá permitir llegar al lanzamiento con evidencia de que ZAREVOA:

- Funciona técnicamente.
- Personaliza realmente.
- Genera rutas razonables.
- Maneja errores.
- Protege información.
- Puede utilizarse cómodamente desde móvil.
- Está preparada para aprender de usuarios reales.

29. Principio final

ZAREVOA no estará lista porque el desarrollo haya terminado.

Estará lista cuando las pruebas demuestren que una persona real puede confiar en la experiencia para construir un viaje coherente, personalizado y útil.
