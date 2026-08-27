# ZAREVOA — Plan de Pruebas y Control de Calidad

## 1. Propósito

Este documento define el sistema inicial de pruebas y control de calidad de ZAREVOA.

El objetivo es asegurar que cada versión del producto funcione correctamente antes de llegar a los usuarios y, especialmente, que las rutas e itinerarios generados sean coherentes, realistas y útiles.

En ZAREVOA, calidad no significa únicamente que la aplicación funcione técnicamente.

También significa que **la planificación tenga sentido para el viajero**.

---

## 2. Principio de calidad

ZAREVOA deberá validar tres dimensiones principales:

### Calidad técnica

La plataforma funciona correctamente.

### Calidad de planificación

Las rutas, tiempos, bases, actividades y presupuestos son razonables.

### Calidad de experiencia

El usuario comprende el proceso y puede utilizarlo sin dificultad innecesaria.

Las tres dimensiones deberán funcionar conjuntamente.

---

## 3. Estrategia de pruebas

Las pruebas se realizarán progresivamente durante el desarrollo.

No se esperará hasta el final para comprobar si ZAREVOA funciona.

El ciclo será:

**Construir → probar → detectar → corregir → volver a probar.**

Cada funcionalidad importante deberá ser validada antes de considerarse terminada.

---

## 4. Pruebas del flujo principal

El recorrido fundamental de ZAREVOA deberá probarse de principio a fin:

1. Entrada a ZAREVOA.
2. Inicio de una planificación.
3. Creación del Travel Profile.
4. Definición de preferencias.
5. Generación de la ruta recomendada.
6. Visualización de “Tu ruta recomendada”.
7. Modificación de la ruta cuando corresponda.
8. Aprobación.
9. Generación del itinerario.
10. Visualización del resultado.

Este flujo tendrá prioridad sobre funcionalidades secundarias.

---

## 5. Pruebas del Travel Profile

Se deberá comprobar que:

- Las preguntas sean comprensibles.
- Las opciones sean suficientes.
- No existan preguntas innecesarias.
- Los campos obligatorios estén claramente identificados.
- Las respuestas se guarden correctamente.
- El usuario pueda avanzar y retroceder.
- Las preferencias lleguen correctamente al ZAREVOA Engine.
- Las modificaciones posteriores se reflejen en la planificación.

También se deberá medir dónde abandonan los usuarios el formulario.

---

## 6. Perfiles de prueba

ZAREVOA deberá probarse utilizando diferentes tipos de viajes.

Ejemplos:

### Viajero individual

- Viaje corto.
- Presupuesto económico.
- Ritmo intenso.
- Intereses específicos.

### Pareja

- Duración media.
- Presupuesto equilibrado.
- Ritmo relajado.
- Intereses compartidos y diferentes.

### Familia

- Diferentes edades.
- Ritmo equilibrado.
- Menor cantidad de cambios de alojamiento.
- Actividades compatibles con las preferencias declaradas.

### Grupo

- Diferentes intereses.
- Presupuesto definido.
- Necesidad de equilibrar preferencias.

El objetivo no será asumir cómo debe viajar cada grupo, sino comprobar que ZAREVOA responde correctamente a la información entregada.

---

## 7. Pruebas por duración

Se deberán probar al menos:

- Escapadas de 2–3 días.
- Viajes de aproximadamente una semana.
- Viajes de 10–14 días.
- Viajes de varias semanas.

Se observará especialmente si el número de bases propuestas tiene sentido según la duración disponible.

ZAREVOA deberá evitar itinerarios excesivamente fragmentados.

---

## 8. Pruebas de ritmo

Cada viaje deberá probarse con los tres ritmos definidos:

### Relajado

Menor cantidad de actividades y mayor margen de tiempo.

### Equilibrado

Combinación razonable entre actividades y tiempo libre.

### Intenso

Mayor aprovechamiento del día sin crear jornadas físicamente o logísticamente absurdas.

Cambiar el ritmo deberá producir diferencias reales en la planificación.

---

## 9. Pruebas de presupuesto

Se deberán probar:

- Económico.
- Equilibrado.
- Confort.
- Premium.
- Presupuesto total definido por el usuario.

El sistema deberá comprobar si el presupuesto es compatible con la ruta propuesta.

Cuando exista una incompatibilidad importante, ZAREVOA deberá informar o adaptar la planificación en lugar de ignorar la restricción.

---

## 10. Pruebas de intereses

Se deberán crear perfiles con diferentes combinaciones:

- Cultura.
- Historia.
- Gastronomía.
- Naturaleza.
- Aventura.
- Playas.
- Vida urbana.
- Compras.
- Fotografía.
- Experiencias locales.
- Otros intereses incorporados posteriormente.

Las recomendaciones “For You” deberán cambiar de forma perceptible según los intereses seleccionados.

---

## 11. Pruebas de “Must See” y “For You”

Se deberá comprobar que:

### Must See

Representa lugares o experiencias especialmente relevantes dentro del destino.

### For You

Representa recomendaciones vinculadas específicamente con el Travel Profile.

Las dos categorías no deberán convertirse simplemente en listas genéricas de lugares populares.

---

## 12. Pruebas de bases

La selección de bases será una de las funciones más importantes del ZAREVOA Engine.

Se deberá comprobar:

- Número de bases.
- Distancia entre bases.
- Tiempo necesario para cambiar de alojamiento.
- Duración de permanencia en cada base.
- Utilidad real de cada cambio.
- Relación entre duración total y cantidad de bases.

Cada cambio de alojamiento deberá aportar suficiente valor para justificar el tiempo y esfuerzo que implica.

---

## 13. Pruebas de transición

Los tiempos de transición deberán considerar más que el tiempo puro de transporte.

Cuando corresponda se deberá contemplar:

- Preparación.
- Check-out.
- Traslado a estación o aeropuerto.
- Espera.
- Transporte.
- Recogida de equipaje.
- Traslado al nuevo alojamiento.
- Check-in.
- Margen razonable.

Los días de transición deberán tener una carga de actividades menor.

---

## 14. Pruebas de llegada y salida

Los días de llegada y salida requieren tratamiento especial.

Se deberá comprobar que:

- No existan actividades imposibles después de un vuelo.
- Se considere la hora real de llegada cuando esté disponible.
- Exista margen para controles y equipaje.
- El día de salida no tenga actividades incompatibles con el horario del transporte.
- Los vuelos nocturnos o tempranos se manejen correctamente.

---

## 15. Pruebas de modificación de ruta

Una función esencial será modificar una ruta sin comenzar nuevamente.

Se deberá probar:

- Agregar una base.
- Eliminar una base.
- Cambiar cantidad de días.
- Cambiar orden de destinos.
- Cambiar ritmo.
- Cambiar presupuesto.
- Cambiar intereses.

El sistema deberá conservar la información que siga siendo válida.

No deberá regenerar innecesariamente todo el viaje.

---

## 16. Pruebas de datos reales

Cuando ZAREVOA utilice información externa se deberá verificar:

- Distancias.
- Tiempos.
- Ubicaciones.
- Horarios.
- Precios cuando estén disponibles.
- Información de transporte.
- Datos de lugares.
- Información sensible al tiempo.

Las pruebas deberán detectar diferencias importantes entre los datos utilizados por ZAREVOA y la realidad.

---

## 17. Pruebas de APIs

Cada integración deberá probar:

- Respuesta correcta.
- Respuesta vacía.
- Error.
- Tiempo de espera.
- Límite de consultas.
- Datos incompletos.
- Cambio inesperado de formato.
- Servicio temporalmente no disponible.

ZAREVOA deberá manejar estos casos sin mostrar errores incomprensibles al usuario.

---

## 18. Pruebas de inteligencia artificial

Se deberá comprobar:

- Consistencia.
- Cumplimiento de reglas ZAREVOA.
- Formato de respuesta.
- Información inventada.
- Interpretación de preferencias.
- Variaciones excesivas entre resultados similares.
- Coste por ejecución.
- Tiempo de respuesta.

La salida de la IA deberá validarse antes de convertirse en información estructural del itinerario cuando sea necesario.

---

## 19. Pruebas de interfaz

Se deberá probar ZAREVOA en:

- Teléfonos móviles.
- Tablets cuando sea relevante.
- Computadores.
- Diferentes resoluciones.
- Navegadores principales.

Comprobar:

- Textos legibles.
- Botones accesibles.
- Formularios utilizables.
- Navegación.
- Mapas.
- Tarjetas.
- Imágenes.
- Mensajes de error.
- Estados de carga.

La experiencia móvil tendrá especial importancia.

---

## 20. Pruebas de rendimiento

Se medirán:

- Tiempo de carga inicial.
- Tiempo de respuesta.
- Tiempo de generación de ruta.
- Tiempo de generación de itinerario.
- Rendimiento con conexiones lentas.
- Uso de recursos.

Los procesos que requieran más tiempo deberán comunicar claramente al usuario que se encuentran en ejecución.

---

## 21. Pruebas de seguridad

Antes del lanzamiento se comprobará al menos:

- HTTPS.
- Protección de claves API.
- Gestión de sesiones.
- Autorización.
- Validación de entradas.
- Protección de datos personales.
- Dependencias actualizadas.
- Manejo seguro de errores.
- Respaldos.
- Recuperación básica ante incidentes.

Las credenciales nunca deberán aparecer en código público o repositorios.

---

## 22. Pruebas de pagos

Cuando se active monetización se deberá probar:

- Compra correcta.
- Pago rechazado.
- Pago duplicado.
- Interrupción durante el proceso.
- Confirmación.
- Registro de transacción.
- Cancelación.
- Reembolso cuando corresponda.

Se utilizarán entornos de prueba de los proveedores antes de activar pagos reales.

---

## 23. Pruebas de afiliados

Se deberá comprobar:

- Enlaces correctos.
- Parámetros de seguimiento.
- Destino correcto.
- Funcionamiento móvil.
- Identificación de opciones reservables.
- Transparencia comercial.

La existencia de un enlace de afiliado no deberá cambiar artificialmente la recomendación del ZAREVOA Engine.

---

## 24. Pruebas con usuarios reales

Antes del lanzamiento amplio se realizarán pruebas con un grupo reducido de personas.

Se observará:

- Qué entienden sin explicación.
- Dónde dudan.
- Qué preguntas realizan.
- Qué abandonan.
- Qué modifican.
- Qué valoran.
- Qué consideran innecesario.

Siempre que sea posible se observará el comportamiento antes de explicar cómo utilizar la plataforma.

---

## 25. Clasificación de errores

Los errores podrán clasificarse inicialmente como:

### Crítico

Impide completar la planificación, compromete seguridad o genera información gravemente incorrecta.

### Alto

Afecta significativamente una función principal.

### Medio

Existe una alternativa o el problema afecta parcialmente la experiencia.

### Bajo

Problema visual, textual o secundario que no impide utilizar el producto.

Los errores críticos deberán resolverse antes del lanzamiento.

---

## 26. Registro de incidencias

Cada incidencia relevante deberá registrar:

- Descripción.
- Fecha.
- Versión.
- Pasos para reproducirla.
- Resultado esperado.
- Resultado obtenido.
- Evidencia cuando corresponda.
- Nivel de prioridad.
- Estado.
- Solución aplicada.

Esto permitirá evitar que problemas conocidos se pierdan o reaparezcan sin control.

---

## 27. Pruebas de regresión

Cuando se modifique una función importante se deberán volver a probar las funciones relacionadas.

Una mejora no deberá romper algo que anteriormente funcionaba.

Las áreas críticas del flujo principal deberán contar progresivamente con pruebas automatizadas.

---

## 28. Criterios mínimos antes del lanzamiento

ZAREVOA V1 podrá avanzar a lanzamiento cuando:

- El flujo principal pueda completarse.
- No existan errores críticos conocidos.
- El Travel Profile funcione correctamente.
- La ruta recomendada tenga coherencia.
- La modificación de ruta funcione.
- Los itinerarios sean razonables.
- Los tiempos de transición estén considerados.
- Las integraciones esenciales sean estables.
- La experiencia móvil sea funcional.
- La seguridad básica esté implementada.
- Existan mecanismos para detectar errores después del lanzamiento.

---

## 29. Control de calidad después del lanzamiento

Después del lanzamiento se deberá continuar observando:

- Errores.
- Feedback.
- Abandonos.
- Modificaciones de rutas.
- Regeneraciones.
- Rendimiento.
- Costes.
- Problemas con proveedores.
- Incidentes de seguridad.

La calidad será un proceso permanente.

---

## 30. Principio final

ZAREVOA no deberá evaluar únicamente si una función técnicamente funciona.

La pregunta más importante será:

**¿El resultado tiene sentido para una persona que realmente realizará este viaje?**

El control de calidad de ZAREVOA deberá proteger precisamente eso:

**la confianza del viajero en que la planificación recibida es coherente, realista y útil.**
