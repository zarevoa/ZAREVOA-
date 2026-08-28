137 — PROTOCOLO DE CONTROL DE VERSIONES ZAREVOA V1

1. Objetivo

Establecer un sistema simple y ordenado para identificar, registrar y controlar las distintas versiones de ZAREVOA durante su desarrollo, pruebas y lanzamiento.

El propósito es saber con claridad qué versión está funcionando, qué cambios contiene y permitir recuperar una versión anterior cuando sea necesario.

2. Principio general

Cada cambio relevante realizado en ZAREVOA deberá quedar asociado a una versión identificable.

El control de versiones permitirá evitar confusiones entre archivos, código, configuraciones y funcionalidades correspondientes a diferentes etapas del proyecto.

3. Sistema de versiones

ZAREVOA utilizará inicialmente una numeración del tipo:

V1.0.0

Los números representarán:

Primer número — Versión principal

Cambios importantes o nuevas etapas del producto.

Segundo número — Versión funcional

Nuevas funcionalidades o mejoras relevantes compatibles con la versión principal.

Tercer número — Corrección

Correcciones de errores o ajustes menores.

Ejemplos:

- V1.0.0 — Primera versión pública.
- V1.1.0 — Nueva funcionalidad relevante.
- V1.1.1 — Corrección de errores.
- V2.0.0 — Nueva generación importante del producto.

4. Versiones durante desarrollo

Antes del lanzamiento podrán utilizarse identificadores complementarios como:

- Alpha.
- Beta.
- Release Candidate.

Ejemplos:

V1.0.0-alpha

V1.0.0-beta

V1.0.0-rc

Esto permitirá diferenciar claramente una versión de pruebas de una versión pública estable.

5. Alpha

La etapa Alpha corresponderá a versiones tempranas utilizadas principalmente para desarrollo y pruebas internas.

Podrán contener:

- Funciones incompletas.
- Errores conocidos.
- Cambios frecuentes.
- Datos o integraciones provisionales.

No deberán considerarse listas para usuarios generales.

6. Beta

La etapa Beta corresponderá a una versión suficientemente completa para ser utilizada por un grupo controlado de usuarios.

El objetivo será detectar:

- Problemas reales de uso.
- Errores no identificados internamente.
- Dificultades de comprensión.
- Debilidades en las recomendaciones.
- Mejoras necesarias antes del lanzamiento.

7. Release Candidate

Una versión candidata a lanzamiento deberá contener todas las funcionalidades previstas para V1 y no presentar errores críticos conocidos.

Si las pruebas finales son satisfactorias, podrá convertirse en la versión pública sin cambios importantes.

8. Registro de versión

Cada versión relevante deberá registrar, como mínimo:

- Número de versión.
- Fecha.
- Cambios principales.
- Correcciones.
- Funciones incorporadas.
- Problemas conocidos.
- Estado de pruebas.

9. Relación con incidencias

Cuando una versión corrija una incidencia registrada, será conveniente indicar su identificador.

Ejemplo:

V1.0.0-beta.3 — Corrige ZAR-018.

Esto permitirá saber en qué versión se solucionó cada problema.

10. Relación con cambios

Las modificaciones aprobadas mediante el protocolo de gestión de cambios deberán asociarse a la versión donde fueron implementadas.

Así podrá conocerse qué comportamiento corresponde a cada etapa del producto.

11. Código fuente

El código deberá mantenerse en un sistema de control de versiones adecuado.

Cada cambio importante deberá conservar suficiente trazabilidad para identificar:

- Qué se modificó.
- Cuándo.
- Por qué.
- Quién realizó el cambio cuando participen varias personas.

12. Commits

Los commits deberán utilizar mensajes suficientemente claros.

Se evitarán mensajes ambiguos como:

- cambios.
- arreglo.
- prueba.
- varias cosas.

Será preferible utilizar descripciones como:

Corrige cálculo de días de traslado.

Añade modificación de ruta sin reiniciar Travel Profile.

Ajusta visualización móvil del itinerario.

13. Ramas de trabajo

Cuando el desarrollo lo requiera podrán utilizarse ramas separadas para:

- Nuevas funcionalidades.
- Correcciones.
- Pruebas.
- Producción.

La estructura deberá mantenerse tan sencilla como permita el tamaño real del proyecto.

14. Versión estable

Deberá existir siempre una referencia clara de cuál es la última versión considerada estable.

No deberán realizarse pruebas experimentales directamente sobre la única versión estable disponible cuando exista riesgo de afectar el servicio.

15. Despliegue

Antes de publicar una nueva versión deberá comprobarse:

1. Qué cambios contiene.
2. Qué pruebas fueron realizadas.
3. Si existen incidencias críticas.
4. Si las configuraciones necesarias están preparadas.
5. Si existe posibilidad razonable de reversión.

16. Reversión

Si una nueva versión provoca un problema grave, deberá poder restaurarse la última versión estable cuando sea técnicamente posible.

La reversión deberá considerarse parte del proceso normal de seguridad y no un fracaso del desarrollo.

17. Base de datos

Los cambios estructurales de base de datos deberán gestionarse cuidadosamente.

Antes de modificaciones importantes deberán considerarse:

- Compatibilidad.
- Migraciones.
- Respaldo.
- Recuperación.
- Impacto sobre datos existentes.

18. Integraciones

Cuando cambie una API o proveedor externo deberá registrarse la modificación si afecta el comportamiento del producto.

Esto permitirá identificar posteriormente problemas relacionados con servicios de terceros.

19. Documentación

Las decisiones documentales importantes deberán mantenerse sincronizadas con la versión del producto.

No será necesario crear una copia completa de todos los documentos para cada versión, pero sí deberá poder identificarse qué decisiones están vigentes.

20. Versiones posteriores al lanzamiento

Después de V1.0.0, las nuevas versiones deberán priorizar:

- Correcciones.
- Mejoras basadas en uso real.
- Evolución del ZAREVOA Engine.
- Funciones Post V1 previamente evaluadas.

21. Evitar numeración excesiva

El sistema de versiones deberá servir para aportar claridad y no burocracia.

Los cambios mínimos de texto o ajustes internos podrán agruparse cuando no justifiquen una versión pública independiente.

22. Resultado esperado

El control de versiones permitirá que ZAREVOA pueda evolucionar manteniendo trazabilidad, estabilidad y capacidad de recuperación.

En cualquier momento deberá ser posible saber cuál es la versión estable y qué cambios introdujo una nueva versión.

23. Principio final

Cada versión de ZAREVOA deberá representar un estado identificable y comprobable del producto.

Cambiar, probar, registrar y poder volver atrás permitirá evolucionar con velocidad sin perder control sobre lo que ya funciona.
