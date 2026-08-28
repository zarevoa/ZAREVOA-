138 — PROTOCOLO DE DESPLIEGUE ZAREVOA V1

1. Objetivo

Establecer el procedimiento para publicar nuevas versiones de ZAREVOA de forma controlada, verificable y segura durante las etapas de desarrollo, pruebas y lanzamiento.

El propósito es reducir el riesgo de que una actualización afecte funciones que ya se encuentran operativas.

2. Principio general

Ninguna versión deberá pasar directamente de desarrollo a producción sin una revisión previa proporcional a la importancia de los cambios realizados.

El flujo recomendado será:

Desarrollo → Pruebas → Validación → Despliegue → Verificación → Monitoreo.

3. Entornos

Cuando la arquitectura lo permita, ZAREVOA deberá diferenciar al menos:

Desarrollo

Entorno utilizado para construir y modificar funcionalidades.

Pruebas

Entorno destinado a comprobar integraciones, rutas, itinerarios, errores y nuevas versiones antes de exponerlas a usuarios reales.

Producción

Entorno utilizado por los usuarios reales.

La complejidad de estos entornos podrá crecer junto con el proyecto.

4. Preparación del despliegue

Antes de publicar una nueva versión deberá confirmarse:

- Número de versión.
- Cambios incluidos.
- Incidencias corregidas.
- Pruebas realizadas.
- Configuraciones necesarias.
- Integraciones afectadas.
- Cambios de base de datos.
- Variables de entorno.
- Posibilidad de reversión.

5. Protección de credenciales

Las claves API, tokens, contraseñas y otros secretos no deberán incluirse directamente en el código publicado.

Deberán utilizarse mecanismos adecuados de variables de entorno o gestión de secretos.

6. Pruebas previas

Antes del despliegue se deberán ejecutar las pruebas relacionadas con los cambios.

Cuando se modifique el ZAREVOA Engine deberán repetirse los escenarios relevantes de la matriz de pruebas.

7. Revisión del flujo principal

Antes de una publicación importante deberá comprobarse nuevamente:

Inicio → Travel Profile → ZAREVOA Engine → Tu ruta recomendada → modificación o aprobación → itinerario → guardado y recuperación.

Este recorrido deberá mantenerse operativo.

8. Base de datos

Si el despliegue incluye cambios estructurales en la base de datos se deberá evaluar:

- Migración necesaria.
- Compatibilidad con información existente.
- Respaldo previo.
- Posibilidad de reversión.
- Riesgo de pérdida de datos.

Los cambios destructivos deberán evitarse cuando exista una alternativa más segura.

9. Integraciones externas

Antes de publicar se comprobará que los servicios externos necesarios estén correctamente configurados.

Por ejemplo:

- Mapas.
- Datos de lugares.
- Inteligencia artificial.
- Autenticación.
- Pagos.
- Analítica.
- Afiliados.
- Correo u otros servicios.

10. Despliegues pequeños

Siempre que sea posible se preferirán cambios pequeños y frecuentes frente a grandes publicaciones que mezclen numerosas modificaciones.

Esto facilitará:

- Detectar problemas.
- Identificar causas.
- Revertir cambios.
- Probar resultados.

11. Momento del despliegue

Las actualizaciones importantes deberán realizarse, cuando sea posible, en momentos en que exista capacidad para supervisar el sistema posteriormente.

Se evitará publicar cambios críticos y dejar inmediatamente el sistema sin seguimiento.

12. Verificación posterior

Después de cada despliegue importante se comprobará:

- Acceso a la plataforma.
- Creación de viaje.
- Travel Profile.
- Generación de ruta.
- Generación de itinerario.
- Guardado.
- Recuperación.
- Integraciones principales.
- Errores visibles.

13. Monitoreo

Durante el período posterior al despliegue se observarán especialmente:

- Errores.
- Tiempos de respuesta.
- Fallos de APIs.
- Problemas de autenticación.
- Fallos en generación.
- Incidencias reportadas.
- Comportamientos anormales.

14. Despliegue fallido

Si una versión genera un problema crítico se deberá priorizar la recuperación del servicio.

Según el caso se podrá:

1. Corregir inmediatamente.
2. Desactivar temporalmente la función afectada.
3. Revertir a la última versión estable.

15. Reversión

La posibilidad de volver a una versión estable deberá considerarse antes del despliegue y no después de que ocurra un problema.

Cuando existan cambios de base de datos, la estrategia de reversión deberá evaluarse especialmente.

16. Registro

Cada despliegue relevante deberá registrar:

- Fecha.
- Versión.
- Cambios principales.
- Responsable.
- Resultado.
- Incidencias detectadas.
- Reversión realizada, si correspondió.

17. Despliegue de emergencia

Los problemas críticos de seguridad, pérdida de datos o indisponibilidad podrán requerir una publicación urgente.

Incluso en estos casos se deberá realizar la prueba mínima necesaria antes de publicar la corrección.

18. Primera publicación pública

El lanzamiento de ZAREVOA V1 deberá considerarse un despliegue especialmente controlado.

Antes de abrir el acceso se verificará:

- Flujo principal completo.
- Experiencia móvil.
- Seguridad básica.
- Privacidad.
- Datos reales e integraciones.
- Analítica.
- Sistema de incidencias.
- Capacidad de recuperación.

19. Lanzamiento gradual

Cuando sea conveniente, ZAREVOA podrá abrirse progresivamente:

Equipo interno → usuarios de prueba → beta limitada → lanzamiento público.

Esto permitirá detectar problemas con menor impacto.

20. Comunicación

Cuando una actualización produzca cambios relevantes para los usuarios se evaluará informar de forma sencilla qué mejoró o cambió.

No será necesario comunicar cada modificación técnica interna.

21. Automatización futura

A medida que el proyecto crezca, el proceso podrá incorporar:

- Pruebas automáticas.
- Integración continua.
- Despliegue continuo controlado.
- Verificaciones automáticas.
- Alertas.
- Monitoreo avanzado.

La automatización deberá incorporarse cuando reduzca riesgos y trabajo repetitivo.

22. Resultado esperado

Este protocolo permitirá publicar nuevas versiones de ZAREVOA manteniendo estabilidad y capacidad de respuesta ante problemas.

El despliegue deberá convertirse en un proceso normal y repetible, no en una acción improvisada.

23. Principio final

Publicar una nueva versión no significa únicamente colocar código en producción.

Cada despliegue deberá proteger lo que ya funciona, comprobar lo que cambió y permitir reaccionar rápidamente si algo no sale como estaba previsto.
