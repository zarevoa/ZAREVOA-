136 — PROTOCOLO DE GESTIÓN DE CAMBIOS ZAREVOA V1

1. Objetivo

Establecer un procedimiento para evaluar, aprobar, implementar y documentar cambios durante el desarrollo de ZAREVOA V1.

El propósito es permitir que el proyecto evolucione sin perder coherencia ni ampliar innecesariamente el alcance de la primera versión.

2. Principio general

Durante el desarrollo aparecerán nuevas ideas, mejoras y necesidades.

No todo cambio deberá implementarse inmediatamente.

Antes de incorporarlo se deberá determinar si:

- Resuelve un problema real.
- Es necesario para V1.
- Mejora significativamente la experiencia.
- Afecta otras funciones.
- Aumenta costos o complejidad.
- Puede reservarse para una versión posterior.

3. Tipos de cambios

Los cambios podrán clasificarse como:

Corrección

Soluciona un error o comportamiento incorrecto.

Mejora

Optimiza una función existente sin modificar significativamente su propósito.

Cambio funcional

Modifica la forma en que una función trabaja o añade una capacidad relevante.

Cambio de diseño

Afecta pantallas, navegación, textos o experiencia visual.

Cambio técnico

Modifica arquitectura, infraestructura, integraciones, base de datos o tecnología.

Cambio de negocio

Afecta productos, precios, monetización, afiliados o modelo comercial.

Cambio de seguridad o cumplimiento

Necesario para proteger información, reducir riesgos o cumplir obligaciones aplicables.

4. Registro del cambio

Los cambios relevantes deberán registrarse indicando:

- Qué se propone cambiar.
- Por qué.
- Qué problema resuelve.
- Qué documentos o módulos afecta.
- Prioridad.
- Impacto esperado.
- Decisión final.

Los ajustes menores de texto o formato podrán realizarse sin un proceso excesivamente formal.

5. Evaluación

Antes de aprobar un cambio relevante se deberán responder estas preguntas:

1. ¿Es necesario para V1?
2. ¿Qué valor aporta al viajero?
3. ¿Afecta el flujo principal?
4. ¿Afecta al ZAREVOA Engine?
5. ¿Genera nuevas dependencias?
6. ¿Aumenta costos?
7. ¿Retrasa el lanzamiento?
8. ¿Puede implementarse después de V1?

6. Protección del alcance V1

Una nueva idea no deberá incorporarse automáticamente a la primera versión.

Si una función aporta valor pero no es necesaria para validar el núcleo de ZAREVOA, deberá registrarse como candidata para una versión posterior.

El objetivo será evitar crecimiento descontrolado del alcance.

7. Cambios urgentes

Tendrán prioridad los cambios relacionados con:

- Seguridad.
- Privacidad.
- Pérdida de datos.
- Errores críticos.
- Información engañosa.
- Bloqueos del flujo principal.
- Problemas legales relevantes.

Estos cambios podrán desplazar temporalmente otras prioridades.

8. Impacto transversal

Antes de implementar una modificación deberá analizarse si afecta:

- Travel Profile.
- ZAREVOA Engine.
- Ruta recomendada.
- Itinerario.
- Diseño.
- Base de datos.
- Integraciones.
- Analítica.
- Monetización.
- Documentación.

Un cambio aparentemente pequeño puede producir efectos en varias áreas.

9. Aprobación

Los cambios importantes deberán contar con una decisión clara antes de implementarse.

La aprobación deberá definir si el cambio:

- Se implementa ahora.
- Se programa para una etapa posterior de V1.
- Se reserva para Post V1.
- Se rechaza.

10. Implementación

Los cambios aprobados deberán realizarse de forma controlada.

Siempre que sea posible:

Modificar → probar → comparar → validar → incorporar.

No deberán introducirse múltiples cambios importantes simultáneamente cuando esto dificulte identificar la causa de posibles problemas.

11. Pruebas

Todo cambio que afecte funcionalidades deberá probarse.

Cuando modifique reglas del ZAREVOA Engine se deberán repetir escenarios relacionados de la matriz de pruebas.

12. Regresión

Después de cambios relevantes se comprobará que funciones previamente correctas continúen funcionando.

La corrección de un problema no deberá crear otro de mayor impacto.

13. Actualización documental

Cuando un cambio modifique una decisión oficial, deberán actualizarse los documentos relacionados.

No deberá quedar una especificación antigua contradiciendo el comportamiento real del producto.

14. Cambios temporales

Si se implementa una solución provisional, deberá quedar identificada como tal.

Las soluciones temporales no deberán convertirse accidentalmente en decisiones permanentes por falta de seguimiento.

15. Reversión

Cuando un cambio provoque problemas importantes deberá existir la posibilidad de volver a una versión estable cuando técnicamente corresponda.

Esto será especialmente relevante durante despliegues y modificaciones del Engine.

16. Cambios posteriores al lanzamiento

Después del lanzamiento se mantendrá el mismo principio.

Las solicitudes de usuarios deberán analizarse buscando patrones antes de transformarlas en funciones permanentes.

17. Métricas

Cuando sea posible, las mejoras importantes deberán evaluarse mediante resultados reales.

Por ejemplo:

- Mayor finalización del Travel Profile.
- Menos modificaciones de ruta.
- Mayor guardado de viajes.
- Menos errores.
- Mejor valoración.
- Mayor conversión.

18. Decisiones basadas en evidencia

La opinión seguirá siendo útil durante el desarrollo, pero progresivamente deberá complementarse con:

- Pruebas.
- Datos.
- Incidencias.
- Comentarios de usuarios.
- Resultados de uso.

19. Historial

Los cambios relevantes deberán conservar suficiente trazabilidad para comprender posteriormente:

- Qué cambió.
- Por qué cambió.
- Cuándo.
- Qué decisión reemplazó.

20. Resultado esperado

Este protocolo permitirá mejorar ZAREVOA sin convertir cada nueva idea en una modificación inmediata del producto.

El desarrollo podrá avanzar con flexibilidad, pero manteniendo control sobre alcance, calidad y coherencia.

21. Principio final

ZAREVOA deberá evolucionar constantemente, pero no impulsivamente.

Cada cambio importante deberá tener una razón clara, un impacto comprendido y una mejora verificable para el proyecto o para el viajero.
