134 — MATRIZ DE ESCENARIOS DE PRUEBA ZAREVOA V1

1. Objetivo

Definir un conjunto de escenarios representativos para probar ZAREVOA V1 y comprobar que el sistema responda correctamente ante distintos tipos de viajeros, duraciones, presupuestos, ritmos e intereses.

La matriz permitirá evaluar no solo el funcionamiento técnico, sino también la calidad del criterio utilizado por ZAREVOA.

2. Principio de prueba

Cada escenario deberá comprobar tres aspectos:

1. Funcionamiento: el sistema completa el proceso sin errores.
2. Coherencia: la ruta y el itinerario son realistas.
3. Personalización: el resultado cambia de manera lógica según el perfil.

3. Escenario 01 — Viaje individual corto

Perfil:

- 1 viajero.
- 3 a 4 días.
- Presupuesto equilibrado.
- Ritmo equilibrado.
- Intereses generales.

Validar:

- Pocas bases.
- Traslados mínimos.
- Buena utilización del tiempo.
- Itinerario sin saturación.

4. Escenario 02 — Pareja, ritmo relajado

Perfil:

- 2 viajeros.
- 7 días.
- Presupuesto confort.
- Ritmo relajado.
- Gastronomía, cultura y paseos.

Validar:

- Menor cantidad de actividades diarias.
- Pausas razonables.
- Traslados cómodos.
- Tiempo libre suficiente.

5. Escenario 03 — Pareja, ritmo intenso

Mantener destino y duración similares al escenario anterior, cambiando principalmente el ritmo.

Validar:

- Mayor cantidad razonable de actividades.
- Diferencia perceptible respecto al ritmo relajado.
- Ausencia de horarios imposibles.

6. Escenario 04 — Familia

Perfil:

- Adultos y menores.
- 7 a 10 días.
- Presupuesto equilibrado.
- Intereses variados.

Validar:

- Consideración de la composición del grupo.
- Actividades compatibles con preferencias declaradas.
- Descansos adecuados.
- Ausencia de estereotipos automáticos basados únicamente en edad.

7. Escenario 05 — Grupo de adultos

Perfil:

- 4 a 6 viajeros.
- 8 días.
- Ritmo equilibrado.
- Intereses diversos.

Validar:

- Recomendaciones suficientemente amplias.
- Logística razonable.
- Capacidad de equilibrar intereses.

8. Escenario 06 — Presupuesto económico

Perfil:

- Viaje de duración media.
- Nivel Económico.

Validar:

- Priorización de alternativas compatibles con el presupuesto.
- Evitar recomendaciones premium como opción principal.
- Mantener calidad de experiencia sin convertir el viaje únicamente en búsqueda de menor precio.

9. Escenario 07 — Presupuesto premium

Perfil:

- Duración equivalente al escenario económico.
- Nivel Premium.

Validar:

- Diferencias razonables en alojamiento, experiencias o comodidad.
- Evitar gastos elevados sin valor real.
- Mantener coherencia con los intereses.

10. Escenario 08 — Must See prioritario

Perfil:

- Usuario identifica uno o más lugares como imprescindibles.

Validar:

- Incorporación prioritaria.
- Organización de la ruta alrededor de ellos cuando sea razonable.
- Advertencia cuando exista incompatibilidad real de tiempo o distancia.

11. Escenario 09 — Interés específico

Perfil:

- Interés principal claramente definido, por ejemplo naturaleza, gastronomía, historia, arte o fotografía.

Validar:

- Presencia perceptible del interés en el itinerario.
- Evitar llenar todos los días con actividades idénticas.
- Mantener variedad razonable.

12. Escenario 10 — Múltiples intereses

Perfil:

- Varios intereses con diferentes prioridades.

Validar:

- Ponderación adecuada.
- Mayor presencia de los intereses prioritarios.
- Inclusión razonable de intereses secundarios.

13. Escenario 11 — Viaje de una sola base

Perfil:

- Duración corta o destino adecuado para permanecer en un único alojamiento.

Validar:

- Que el Engine no añada bases innecesarias.
- Excursiones razonables desde la base cuando correspondan.

14. Escenario 12 — Viaje con varias bases

Perfil:

- Duración suficiente.
- Región o país donde varias bases aporten valor.

Validar:

- Orden geográfico.
- Número razonable de cambios.
- Distribución adecuada de noches.
- Traslados realistas.

15. Escenario 13 — Día de llegada

Validar:

- Consideración del tiempo real disponible.
- Traslado desde aeropuerto, estación u otro punto de llegada.
- Actividades ligeras cuando corresponda.
- Evitar una jornada completa ficticia.

16. Escenario 14 — Día de salida

Validar:

- Consideración del horario de salida.
- Tiempo necesario para traslado.
- Margen razonable.
- Evitar actividades incompatibles.

17. Escenario 15 — Traslado entre bases

Validar:

- Duración real del desplazamiento.
- Check-out y check-in cuando sean relevantes.
- Reducción de actividades.
- Evitar tratar el día como jornada turística completa.

18. Escenario 16 — Modificación de ruta

El usuario cambia una base después de recibir la propuesta.

Validar:

- Recalcular elementos afectados.
- Mantener preferencias.
- No reiniciar el Travel Profile.
- Actualizar coherentemente el itinerario posterior.

19. Escenario 17 — Cambio de duración

El usuario añade o elimina días.

Validar:

- Redistribución lógica.
- Evitar simplemente añadir o quitar actividades sin reconsiderar la ruta.

20. Escenario 18 — Cambio de presupuesto

El usuario modifica el nivel de presupuesto después de generar la planificación.

Validar:

- Ajustes relevantes.
- Conservación de la estructura cuando siga siendo válida.
- Cambios en opciones donde realmente corresponda.

21. Escenario 19 — Rechazo de recomendación

El usuario indica que una actividad no le interesa.

Validar:

- Sustitución coherente.
- Evitar volver a recomendar inmediatamente una alternativa prácticamente idéntica.
- Mantener el sentido del día.

22. Escenario 20 — Datos externos no disponibles

Simular fallo de una API o fuente.

Validar:

- Mensaje comprensible.
- No inventar información.
- Conservar el progreso.
- Permitir reintento o alternativa.

23. Escenario 21 — Conexión interrumpida

Simular pérdida temporal de internet.

Validar:

- Evitar pérdida innecesaria del viaje.
- Informar al usuario.
- Recuperar el proceso cuando sea posible.

24. Escenario 22 — Perfil incompleto

El usuario omite información opcional o intenta continuar sin un dato obligatorio.

Validar:

- Identificación clara de campos necesarios.
- No bloquear por información que realmente sea opcional.
- Mensajes simples.

25. Escenario 23 — Destino con poca información

Validar:

- Comportamiento cuando existan pocos datos disponibles.
- Transparencia.
- Evitar completar vacíos mediante información inventada.

26. Escenario 24 — Viaje internacional complejo

Perfil:

- Varias ciudades o países.
- Duración extensa.

Validar:

- Orden de ruta.
- Tiempos de traslado.
- Número de bases.
- Días de transición.
- Evitar recorridos innecesariamente agotadores.

27. Escenario 25 — Comparación de perfiles

Crear dos viajes con:

- Mismo destino.
- Mismas fechas.
- Misma duración.

Cambiar significativamente intereses, ritmo o presupuesto.

Validar:

- Que los resultados no sean prácticamente idénticos.
- Que las diferencias puedan explicarse por el Travel Profile.

28. Registro de resultados

Para cada escenario se deberá registrar:

- Identificador.
- Fecha.
- Versión probada.
- Perfil utilizado.
- Resultado esperado.
- Resultado obtenido.
- Errores encontrados.
- Nivel de gravedad.
- Corrección realizada.
- Estado final.

29. Resultado satisfactorio

Un escenario se considerará aprobado cuando:

- Complete el flujo esperado.
- No presente errores críticos.
- La ruta sea razonable.
- El itinerario sea utilizable.
- La personalización sea coherente.
- Los datos objetivos no se presenten de manera engañosa.

30. Uso continuo

Esta matriz no deberá utilizarse una sola vez.

Los escenarios principales deberán repetirse después de cambios relevantes en el ZAREVOA Engine para comprobar que las mejoras no hayan generado problemas en otros tipos de viaje.

31. Principio final

La calidad del ZAREVOA Engine deberá demostrarse enfrentándolo a viajeros y situaciones diferentes.

Si ZAREVOA comprende realmente al viajero, perfiles diferentes deberán producir viajes diferentes por razones que tengan sentido.
