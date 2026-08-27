# ZAREVOA — Checklist de Lanzamiento V1

## 1. Propósito

Este documento establece el checklist que deberá completarse antes del lanzamiento público de ZAREVOA V1.

Su objetivo es asegurar que la primera versión sea funcional, coherente, segura y suficientemente sólida para comenzar a recibir usuarios reales.

El lanzamiento no requiere que ZAREVOA sea perfecto.

Requiere que su propuesta principal funcione correctamente.

---

## 2. Producto

Antes del lanzamiento deberá comprobarse:

- [ ] La propuesta de valor de ZAREVOA está claramente definida.
- [ ] El alcance de V1 está cerrado.
- [ ] Las funcionalidades futuras están separadas de V1.
- [ ] El flujo principal puede completarse de principio a fin.
- [ ] El usuario entiende qué hace ZAREVOA.
- [ ] El usuario puede comenzar una planificación fácilmente.
- [ ] La experiencia funciona correctamente en dispositivos móviles.
- [ ] La navegación es clara y consistente.
- [ ] No existen pantallas o botones sin función.

---

## 3. Travel Profile

Comprobar que el Travel Profile permite recopilar correctamente la información necesaria para personalizar el viaje.

- [ ] Destino o región de interés.
- [ ] Fechas o duración del viaje.
- [ ] Presupuesto.
- [ ] Nivel de presupuesto.
- [ ] Ritmo de viaje.
- [ ] Intereses.
- [ ] Composición del grupo.
- [ ] Edades cuando sean relevantes.
- [ ] Preferencias importantes.
- [ ] Restricciones indicadas por el usuario.
- [ ] Prioridades personales.

El formulario deberá solicitar únicamente información que tenga utilidad real para la planificación.

---

## 4. ZAREVOA Engine V1

Antes del lanzamiento se deberá validar que el motor:

- [ ] Utiliza datos reales cuando corresponda.
- [ ] Aplica las reglas propias de ZAREVOA.
- [ ] Utiliza IA como apoyo a la planificación.
- [ ] Considera la duración total del viaje.
- [ ] Selecciona bases razonables.
- [ ] Evita exceso de cambios de alojamiento.
- [ ] Considera tiempos reales de transición.
- [ ] Reduce actividades en días de traslado o vuelos.
- [ ] Respeta el ritmo Relajado, Equilibrado o Intenso.
- [ ] Considera el presupuesto disponible.
- [ ] Distribuye el presupuesto de forma adaptable.
- [ ] Prioriza los intereses del viajero.
- [ ] Diferencia recomendaciones “Must See” y “For You”.
- [ ] Considera la composición del grupo sin aplicar estereotipos.
- [ ] Evalúa interés, tiempo y sentido de cada actividad dentro de la ruta.

---

## 5. Ruta recomendada

Antes de generar el itinerario detallado:

- [ ] Se muestra la pantalla “Tu ruta recomendada”.
- [ ] El usuario puede entender fácilmente la ruta.
- [ ] Se muestran las bases principales.
- [ ] Se muestra la distribución de días.
- [ ] Se explican las decisiones importantes cuando sea útil.
- [ ] El usuario puede aprobar la ruta.
- [ ] El usuario puede modificarla.
- [ ] Una modificación no obliga a comenzar nuevamente el formulario.

---

## 6. Itinerario

Comprobar que el itinerario generado:

- [ ] Tiene una secuencia lógica.
- [ ] No contiene jornadas imposibles.
- [ ] Considera distancias y desplazamientos.
- [ ] Considera tiempos de transición.
- [ ] No sobrecarga los días de llegada o salida.
- [ ] Mantiene coherencia con el ritmo elegido.
- [ ] Mantiene coherencia con el presupuesto.
- [ ] Prioriza los intereses seleccionados.
- [ ] Presenta claramente las recomendaciones.
- [ ] Permite distinguir información esencial de información opcional.

---

## 7. Datos e integraciones

Verificar:

- [ ] Las APIs esenciales funcionan correctamente.
- [ ] Existen mecanismos para manejar errores de proveedores externos.
- [ ] No se muestran datos inventados como si fueran información real.
- [ ] La información sensible al tiempo puede identificarse como tal.
- [ ] Las distancias y tiempos utilizados son razonables.
- [ ] Los límites de consumo de APIs están controlados.
- [ ] Existe registro de errores relevantes.
- [ ] La caída de una integración no inutiliza innecesariamente toda la plataforma.

---

## 8. Recomendaciones y afiliados

ZAREVOA deberá mantener claramente separados el criterio de planificación y la monetización.

Comprobar:

- [ ] Una recomendación puede existir aunque no genere comisión.
- [ ] Las opciones reservables se identifican correctamente.
- [ ] Los enlaces de afiliados funcionan.
- [ ] No se presenta una opción comercial como superior únicamente por generar ingresos.
- [ ] Las relaciones comerciales se comunican con transparencia cuando corresponda.
- [ ] El usuario mantiene libertad para reservar donde prefiera.

---

## 9. ZAREVOA Journey y ZAREVOA Personal

Antes de activar productos de pago:

- [ ] Está claramente explicado qué incluye cada producto.
- [ ] El usuario comprende qué obtiene por su pago.
- [ ] Los precios están correctamente mostrados.
- [ ] El proceso de pago funciona.
- [ ] Existe confirmación después del pago.
- [ ] Está definido el proceso de entrega del servicio.
- [ ] Están definidos los límites del acompañamiento ofrecido.
- [ ] No existen promesas que ZAREVOA no pueda cumplir de forma consistente.

---

## 10. Seguridad y privacidad

Antes del lanzamiento:

- [ ] El sitio utiliza HTTPS.
- [ ] Las credenciales y claves API no están expuestas públicamente.
- [ ] Las variables sensibles se almacenan de forma segura.
- [ ] Existe control de acceso cuando corresponda.
- [ ] Se recopilan únicamente los datos necesarios.
- [ ] Existe política de privacidad.
- [ ] Existe política de cookies cuando corresponda.
- [ ] Existe mecanismo para gestionar solicitudes relacionadas con datos personales.
- [ ] Se realizan respaldos de información crítica.
- [ ] Se ha probado el manejo de errores básicos de seguridad.

---

## 11. Legal

Verificar antes de operar públicamente:

- [ ] Términos y condiciones.
- [ ] Política de privacidad.
- [ ] Avisos relacionados con afiliados.
- [ ] Condiciones de compra de productos o servicios.
- [ ] Política de cancelación o devolución cuando corresponda.
- [ ] Información empresarial necesaria.
- [ ] Cumplimiento aplicable según mercados donde opere ZAREVOA.

La documentación legal deberá revisarse profesionalmente cuando el nivel de operación del proyecto lo justifique.

---

## 12. Estructura financiera

Antes de recibir cobros o comisiones:

- [ ] Evaluar estructura empresarial adecuada.
- [ ] Separar finanzas personales y empresariales.
- [ ] Disponer de una cuenta empresarial para operaciones en CLP cuando corresponda.
- [ ] Evaluar una cuenta empresarial en USD.
- [ ] Verificar capacidad de recibir pagos internacionales.
- [ ] Evaluar recepción mediante SWIFT.
- [ ] Evaluar soluciones multidivisa compatibles.
- [ ] Definir sistema de registro de ingresos y gastos.
- [ ] Definir obligaciones tributarias aplicables.

---

## 13. Rendimiento

Realizar pruebas de:

- [ ] Velocidad de carga.
- [ ] Funcionamiento móvil.
- [ ] Diferentes tamaños de pantalla.
- [ ] Navegadores principales.
- [ ] Formularios.
- [ ] Generación de rutas.
- [ ] Generación de itinerarios.
- [ ] Enlaces externos.
- [ ] Errores de conexión.
- [ ] Recuperación ante fallos.

---

## 14. Analítica

Antes del lanzamiento deberán estar disponibles métricas básicas para conocer el comportamiento real de los usuarios.

Medir al menos:

- [ ] Visitas.
- [ ] Inicio de planificación.
- [ ] Travel Profiles completados.
- [ ] Rutas generadas.
- [ ] Rutas aprobadas.
- [ ] Rutas modificadas.
- [ ] Itinerarios generados.
- [ ] Usuarios recurrentes.
- [ ] Conversión hacia productos de pago.
- [ ] Uso de enlaces reservables.
- [ ] Errores y abandonos relevantes.

---

## 15. Pruebas finales

Antes de abrir ZAREVOA al público:

- [ ] Realizar viajes de prueba con diferentes perfiles.
- [ ] Probar viajes cortos.
- [ ] Probar viajes largos.
- [ ] Probar diferentes presupuestos.
- [ ] Probar diferentes ritmos.
- [ ] Probar viajeros individuales.
- [ ] Probar parejas.
- [ ] Probar familias y grupos.
- [ ] Probar modificaciones de ruta.
- [ ] Revisar manualmente itinerarios generados.
- [ ] Corregir errores críticos encontrados.

---

## 16. Criterio para lanzar

ZAREVOA V1 estará preparado para un lanzamiento inicial cuando un usuario pueda:

**Entrar → crear su Travel Profile → recibir una ruta coherente → modificarla si lo desea → aprobarla → obtener un itinerario útil.**

No será necesario tener todas las funcionalidades imaginadas para el futuro.

Será necesario que este recorrido principal funcione bien.

---

## 17. Después del lanzamiento

El lanzamiento no será el final del desarrollo.

Será el comienzo de la validación real.

Después del lanzamiento se deberá:

- Observar.
- Medir.
- Escuchar.
- Corregir.
- Aprender.
- Mejorar.

Las decisiones posteriores deberán basarse cada vez más en el comportamiento y las necesidades reales de los viajeros.

---

## 18. Principio final

ZAREVOA V1 no necesita demostrar todo lo que ZAREVOA podrá llegar a ser.

Necesita demostrar que puede hacer muy bien una cosa:

**entender cómo quiere viajar una persona y convertirlo en un viaje coherente, realista y personalizado.**

Ese será el verdadero punto de partida de ZAREVOA.
