140 — PROTOCOLO DE RESPUESTA A INCIDENTES DE PRODUCCIÓN ZAREVOA

1. Objetivo

Establecer el procedimiento para responder a incidentes que afecten ZAREVOA una vez que la plataforma se encuentre disponible para usuarios reales.

El objetivo será proteger a los viajeros, recuperar el servicio rápidamente, reducir el impacto y aprender de cada incidente.

2. Qué se considera un incidente de producción

Se considerará incidente cualquier situación no planificada que afecte significativamente:

- Disponibilidad.
- Funcionamiento.
- Datos.
- Seguridad.
- Privacidad.
- Pagos.
- Integraciones críticas.
- Generación de rutas o itinerarios.
- Experiencia de una cantidad relevante de usuarios.

3. Principio general

Ante un incidente, el orden de prioridad será:

Proteger al usuario → contener el problema → recuperar el servicio → investigar → corregir → aprender.

No se deberá priorizar la búsqueda inmediata de responsables sobre la recuperación segura del sistema.

4. Niveles de severidad

SEV-1 — Crítico

Ejemplos:

- Plataforma completamente inaccesible.
- Pérdida o exposición significativa de datos.
- Incidente grave de seguridad.
- Pagos incorrectos de forma generalizada.
- Generación sistemática de información potencialmente peligrosa o gravemente engañosa.

Requiere atención inmediata.

SEV-2 — Alto

Ejemplos:

- Una función principal no está disponible.
- Muchos usuarios no pueden generar viajes.
- Una integración esencial falla.
- Problemas importantes de autenticación o guardado.

SEV-3 — Medio

Problema que afecta parcialmente la experiencia pero permite continuar utilizando las funciones esenciales.

SEV-4 — Bajo

Problemas menores sin impacto significativo sobre la operación principal.

5. Detección

Un incidente podrá detectarse mediante:

- Monitoreo automático.
- Alertas.
- Registros técnicos.
- Reportes de usuarios.
- Analítica.
- Proveedores externos.
- Revisión interna.

6. Confirmación inicial

Una vez detectado un posible incidente se deberá comprobar:

1. Qué está ocurriendo.
2. Desde cuándo.
3. Qué funciones están afectadas.
4. Cuántos usuarios podrían estar involucrados.
5. Si continúa activo.
6. Si existe riesgo de seguridad, privacidad o pérdida de datos.

7. Contención

Cuando sea necesario se podrán aplicar medidas como:

- Desactivar temporalmente una función.
- Suspender una integración.
- Revocar una credencial.
- Limitar accesos.
- Revertir una versión.
- Detener temporalmente un proceso automatizado.

La prioridad será evitar que el impacto continúe aumentando.

8. Recuperación

Después de contener el incidente se deberá restaurar el servicio de la forma más segura posible.

Según el caso podrá utilizarse:

- Corrección inmediata.
- Reversión.
- Restauración desde respaldo.
- Cambio temporal de proveedor.
- Desactivación controlada de una función no esencial.

9. Verificación

Antes de considerar recuperado el servicio se deberá comprobar:

- Que la función afectada vuelva a operar.
- Que el flujo principal continúe funcionando.
- Que los datos estén consistentes.
- Que el problema no continúe reproduciéndose.
- Que no se hayan generado nuevos errores importantes.

10. Comunicación al usuario

Cuando un incidente tenga impacto visible o relevante, ZAREVOA deberá comunicarlo de manera:

- Clara.
- Breve.
- Transparente.
- Sin especulaciones.
- Sin ocultar información necesaria.

No será necesario comunicar públicamente cada error técnico menor.

11. Seguridad y privacidad

Cuando exista una posible exposición de datos o acceso no autorizado, el incidente deberá tratarse con prioridad especial.

Se deberán conservar evidencias y evaluar las obligaciones legales de notificación que correspondan según los usuarios y territorios afectados.

12. Pagos

Cuando un incidente afecte cobros o transacciones se deberá identificar:

- Usuarios afectados.
- Operaciones realizadas.
- Duplicidades.
- Cobros incorrectos.
- Reembolsos necesarios.

No se deberán modificar registros financieros sin trazabilidad.

13. Servicios externos

Si la causa corresponde a un proveedor externo, ZAREVOA deberá:

- Confirmar el fallo.
- Determinar qué funciones dependen del servicio.
- Aplicar una alternativa cuando exista.
- Informar al usuario cuando el impacto lo justifique.
- Registrar el incidente.

14. ZAREVOA Engine

Si el incidente corresponde a generación sistemática de rutas o itinerarios incorrectos, se podrá:

- Suspender temporalmente la generación afectada.
- Revertir reglas recientes.
- Limitar determinados escenarios.
- Corregir el Engine.
- Repetir la matriz de pruebas relacionada.

15. Registro del incidente

Cada incidente relevante deberá documentar:

- Identificador.
- Fecha y hora.
- Severidad.
- Versión.
- Funciones afectadas.
- Impacto.
- Causa, cuando se determine.
- Acciones realizadas.
- Tiempo de recuperación.
- Solución definitiva.
- Medidas preventivas.

16. Línea de tiempo

Para incidentes importantes será conveniente conservar una cronología simple:

detección → confirmación → contención → recuperación → resolución.

Esto permitirá posteriormente comprender la respuesta y mejorarla.

17. Investigación de causa

Después de recuperar el servicio se deberá analizar por qué ocurrió el incidente.

El objetivo será encontrar la causa real y no únicamente el síntoma visible.

18. Revisión posterior

Los incidentes relevantes deberán generar una revisión posterior que responda:

- ¿Qué ocurrió?
- ¿Por qué ocurrió?
- ¿Cómo se detectó?
- ¿Qué funcionó bien en la respuesta?
- ¿Qué dificultó la recuperación?
- ¿Qué debemos cambiar?

19. Acciones preventivas

La revisión podrá generar acciones como:

- Nueva prueba automática.
- Nueva alerta.
- Cambio de arquitectura.
- Mejora de respaldo.
- Modificación del Engine.
- Cambio de proveedor.
- Actualización documental.
- Mejora de seguridad.

20. Responsabilidades futuras

Cuando ZAREVOA cuente con un equipo mayor deberán definirse responsables específicos para:

- Coordinación del incidente.
- Tecnología.
- Seguridad.
- Comunicación.
- Operación.

En V1 el sistema podrá mantenerse simple, pero las funciones deberán estar claras.

21. Evidencia y confidencialidad

La información de incidentes deberá protegerse cuando contenga:

- Datos personales.
- Vulnerabilidades.
- Credenciales.
- Información financiera.
- Información interna sensible.

22. Cierre

Un incidente se considerará cerrado cuando:

1. El servicio esté estable.
2. El impacto haya sido controlado.
3. Los usuarios afectados hayan sido atendidos cuando corresponda.
4. La causa haya sido investigada suficientemente.
5. Existan acciones preventivas cuando sean necesarias.
6. La documentación haya sido actualizada.

23. Resultado esperado

Este protocolo permitirá que ZAREVOA pueda reaccionar de manera organizada ante problemas reales sin depender de decisiones improvisadas durante momentos de presión.

24. Principio final

Los incidentes tecnológicos no siempre podrán evitarse.

La diferencia estará en detectarlos pronto, proteger al viajero, recuperar el servicio con rapidez y utilizar cada problema para hacer ZAREVOA más confiable.
