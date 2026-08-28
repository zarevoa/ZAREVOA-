135 — PROTOCOLO DE REGISTRO DE INCIDENCIAS ZAREVOA V1

1. Objetivo

Establecer un procedimiento simple y uniforme para registrar, clasificar, investigar, corregir y cerrar los problemas detectados durante el desarrollo y las pruebas de ZAREVOA V1.

El propósito es evitar que errores importantes queden solamente en conversaciones, mensajes o recuerdos sin seguimiento.

2. Qué se considera una incidencia

Se considerará incidencia cualquier comportamiento que:

- Impida completar una función.
- Produzca un resultado incorrecto.
- Genere una ruta o itinerario incoherente.
- Cause pérdida de información.
- Muestre datos incorrectos o engañosos.
- Afecte la seguridad o privacidad.
- Dificulte significativamente la experiencia.
- No corresponda con una decisión oficial de ZAREVOA.

3. Tipos de incidencia

Las incidencias podrán clasificarse inicialmente como:

Técnica

Errores de programación, infraestructura, base de datos, integración o funcionamiento.

Funcional

Una función no se comporta según lo definido.

Criterio ZAREVOA

El sistema funciona técnicamente, pero la recomendación, ruta o itinerario no tiene suficiente sentido.

Datos

Información incorrecta, incompleta, desactualizada o no verificable.

Experiencia de usuario

Problemas de comprensión, navegación, diseño o interacción.

Seguridad y privacidad

Problemas relacionados con acceso, exposición de datos, credenciales o tratamiento de información.

Contenido

Errores de textos, traducciones, mensajes o información mostrada al usuario.

4. Información mínima del registro

Cada incidencia deberá incluir, cuando corresponda:

- Identificador.
- Fecha.
- Versión.
- Módulo afectado.
- Descripción.
- Pasos para reproducir.
- Resultado esperado.
- Resultado obtenido.
- Evidencia disponible.
- Nivel de gravedad.
- Estado.
- Responsable.
- Solución aplicada.

5. Identificador

Cada incidencia deberá disponer de un código único.

Ejemplo:

ZAR-001

La numeración permitirá hacer seguimiento sin depender únicamente del título del problema.

6. Evidencia

Siempre que sea útil se podrá adjuntar:

- Captura de pantalla.
- Video.
- Mensaje de error.
- Registro técnico.
- Datos del escenario utilizado.
- Resultado generado por el Engine.

La evidencia deberá permitir comprender el problema sin almacenar innecesariamente datos personales.

7. Gravedad

Crítica

Problema que:

- Impide completar el flujo principal.
- Provoca pérdida grave de información.
- Expone datos.
- Compromete seguridad.
- Genera resultados peligrosamente incorrectos.

Deberá atenderse antes del lanzamiento.

Alta

Afecta significativamente una función importante o produce resultados claramente incorrectos.

Deberá priorizarse.

Media

Afecta la experiencia, pero existe una alternativa razonable y el flujo puede continuar.

Baja

Problema menor de presentación, redacción, comodidad o comportamiento no esencial.

8. Prioridad

La prioridad podrá considerar no solo gravedad, sino también:

- Cantidad de usuarios afectados.
- Frecuencia.
- Impacto comercial.
- Impacto en confianza.
- Facilidad de corrección.
- Dependencias con otras funciones.

Una incidencia frecuente de gravedad media puede requerir atención antes que una incidencia alta extremadamente excepcional.

9. Estados

Cada incidencia podrá pasar por los siguientes estados:

Nueva → Revisada → Priorizada → En corrección → En prueba → Resuelta → Cerrada.

También podrá marcarse como:

- No reproducible.
- Duplicada.
- Pospuesta.
- No corresponde.

10. Reproducción

Antes de modificar el sistema deberá intentarse reproducir el problema.

Se deberá identificar:

- Qué hizo el usuario.
- Con qué datos.
- En qué dispositivo o entorno.
- Qué ocurrió.
- Si sucede siempre o solo algunas veces.

11. Incidencias del ZAREVOA Engine

Cuando el problema sea una mala recomendación, no deberá registrarse simplemente como “la ruta está mal”.

Deberá especificarse el motivo.

Por ejemplo:

- Demasiadas bases.
- Traslado excesivo.
- Día saturado.
- Must See ignorado.
- Presupuesto mal interpretado.
- Interés poco representado.
- Recomendación fuera de ruta.
- Tiempo insuficiente.
- Actividad incompatible.

Esto permitirá mejorar reglas concretas.

12. Corrección

Toda corrección deberá intentar resolver la causa y no solamente ocultar el síntoma.

Cuando el cambio afecte una regla general del Engine, deberá evaluarse su impacto sobre otros escenarios.

13. Prueba posterior

Una incidencia no se considerará resuelta únicamente porque se haya modificado el código.

Deberá repetirse el escenario que produjo el problema y confirmar que el resultado esperado se cumple.

14. Regresión

Después de corregir problemas importantes deberán ejecutarse pruebas relacionadas para comprobar que la solución no haya generado nuevos errores.

15. Incidencias duplicadas

Cuando varios registros correspondan al mismo problema, deberán vincularse a una incidencia principal.

Esto permitirá conocer la frecuencia sin realizar varias correcciones independientes.

16. Incidencias de usuarios reales

Durante pruebas beta o después del lanzamiento deberá facilitarse una forma sencilla de recibir problemas reportados por usuarios.

La descripción del usuario podrá transformarse internamente en un registro técnico más estructurado.

17. Información sensible

Los registros de incidencias no deberán contener:

- Contraseñas.
- Tokens.
- Claves API.
- Datos financieros completos.
- Información personal innecesaria.

Cuando una evidencia incluya información sensible deberá ocultarse antes de compartirla.

18. Incidencias de seguridad

Los problemas de seguridad o privacidad deberán tratarse con prioridad especial.

Su información podrá limitarse únicamente a las personas que necesiten intervenir en la solución.

19. Revisión periódica

Durante el desarrollo deberán revisarse regularmente:

- Incidencias abiertas.
- Problemas críticos.
- Errores repetidos.
- Áreas con mayor número de fallos.
- Problemas pospuestos.

Esto permitirá detectar patrones y no solamente corregir casos individuales.

20. Cierre

Una incidencia podrá cerrarse cuando:

1. Se haya comprendido el problema.
2. Se haya aplicado una solución o decisión.
3. La corrección haya sido probada.
4. No exista un error crítico relacionado pendiente.
5. La documentación se haya actualizado cuando corresponda.

21. Aprendizaje

Las incidencias no deberán considerarse únicamente fallos.

También serán una fuente de información para mejorar:

- Reglas del Engine.
- Diseño.
- Preguntas del Travel Profile.
- Integraciones.
- Contenido.
- Procesos internos.

22. Principio final

Cada problema detectado deberá convertirse en conocimiento útil para ZAREVOA.

Registrar, comprender, corregir y comprobar será siempre mejor que solucionar informalmente un error y olvidar por qué ocurrió.
