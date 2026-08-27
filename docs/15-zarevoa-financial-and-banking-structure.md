# 15 — ZAREVOA Financial & Banking Structure

## Estado
Pendiente de implementación.

## Objetivo

Definir una estructura financiera y bancaria clara, segura y escalable para ZAREVOA, separando completamente las finanzas personales de las operaciones comerciales del proyecto.

La estructura deberá estar preparada para operar inicialmente desde Chile y permitir posteriormente recibir ingresos desde distintos países y monedas.

---

## 1. Principio fundamental

ZAREVOA deberá operar con una estructura financiera independiente de las cuentas personales de sus fundadores.

Los ingresos, gastos, comisiones, pagos a proveedores, suscripciones tecnológicas y demás movimientos asociados al negocio deberán registrarse y administrarse desde cuentas destinadas exclusivamente a ZAREVOA.

---

## 2. Estructura bancaria inicial

Antes de activar cobros comerciales, se deberá evaluar la apertura de:

- Cuenta bancaria empresarial en CLP.
- Cuenta bancaria empresarial en USD.
- Capacidad para recibir transferencias internacionales.
- Acceso a transferencias mediante red SWIFT cuando corresponda.
- Tarjeta empresarial para gastos operacionales y tecnológicos.

La elección definitiva del banco deberá considerar costos, seguridad, integración con plataformas de pago y facilidad para operaciones internacionales.

---

## 3. Cuenta multidivisa internacional

ZAREVOA evaluará incorporar una solución financiera multidivisa internacional compatible con empresas constituidas en Chile.

Su finalidad será facilitar:

- Recepción de pagos internacionales.
- Conversión entre monedas.
- Pago de servicios y proveedores extranjeros.
- Administración de ingresos provenientes de distintos mercados.
- Reducción de costos asociados a conversiones y transferencias internacionales.

Esta solución será complementaria a la estructura bancaria empresarial principal.

---

## 4. Fuentes de ingresos

La arquitectura financiera deberá permitir identificar separadamente los ingresos provenientes de:

### ZAREVOA Planner
Ingresos asociados a servicios o funcionalidades de planificación cuando corresponda.

### ZAREVOA Journey
Ingresos provenientes de planes, funcionalidades o servicios premium asociados al viaje.

### ZAREVOA Personal
Ingresos provenientes de servicios personalizados o de mayor nivel de acompañamiento.

### Afiliados y comisiones
Ingresos generados por reservas o derivaciones hacia terceros, incluyendo potencialmente:

- Alojamientos.
- Actividades y experiencias.
- Transporte.
- Seguros de viaje.
- Alquiler de vehículos.
- Otros servicios turísticos compatibles con ZAREVOA.

Las recomendaciones de ZAREVOA deberán mantener independencia de criterio: la existencia de una comisión nunca deberá convertir automáticamente una opción en la recomendación principal.

---

## 5. Pasarelas de pago

Antes del lanzamiento comercial se deberán evaluar proveedores capaces de procesar pagos nacionales e internacionales.

Los criterios principales serán:

- Disponibilidad para empresas chilenas.
- Cobertura internacional.
- Monedas aceptadas.
- Comisiones por transacción.
- Costos de conversión.
- Plazos de liquidación.
- Gestión de devoluciones.
- Protección contra fraude.
- Integración técnica mediante API.
- Experiencia de pago simple para el usuario.

La arquitectura tecnológica deberá evitar una dependencia innecesaria de un único proveedor.

---

## 6. Contabilidad y trazabilidad

Todos los movimientos financieros deberán ser trazables.

Como mínimo se deberá mantener registro de:

- Ingresos.
- Gastos operacionales.
- Comisiones.
- Suscripciones.
- Servicios tecnológicos.
- Marketing.
- Pagos a proveedores.
- Reembolsos.
- Impuestos.
- Costos asociados a procesamiento de pagos.

La estructura contable deberá permitir conocer el costo real de operación y la rentabilidad de cada línea de negocio.

---

## 7. Control financiero

ZAREVOA deberá monitorear progresivamente indicadores como:

- Ingresos mensuales.
- Gastos mensuales.
- Margen operacional.
- Ingreso promedio por usuario.
- Costo de adquisición de clientes.
- Conversión de usuarios gratuitos a servicios pagados.
- Ingresos por afiliación.
- Costos tecnológicos por usuario.
- Tasa de reembolsos.

Durante la etapa inicial se priorizará una estructura simple y de bajo costo.

---

## 8. Separación entre recomendación e ingreso

ZAREVOA deberá preservar uno de sus principios centrales:

> Primero recomendar lo que tiene sentido para el viajero; después determinar si esa opción puede reservarse o generar una comisión.

El motor de planificación no deberá alterar artificialmente una ruta, actividad, alojamiento o servicio únicamente porque genere mayores ingresos para ZAREVOA.

Cuando sea necesario, la relación comercial o de afiliación deberá comunicarse de forma transparente.

---

## 9. Seguridad financiera

La operación financiera deberá aplicar medidas básicas de seguridad, incluyendo:

- Autenticación multifactor.
- Accesos limitados según responsabilidad.
- Registro de operaciones.
- Protección de credenciales.
- Revisión periódica de movimientos.
- Alertas ante operaciones inusuales.
- Respaldo de documentación financiera.

ZAREVOA evitará almacenar directamente información completa de tarjetas bancarias cuando pueda delegarse de forma segura a proveedores especializados de pago.

---

## 10. Implementación por etapas

### Etapa 1 — Desarrollo
Sin necesidad de una infraestructura bancaria compleja.

Prioridad:
producto, tecnología, validación y estructura documental.

### Etapa 2 — Preparación comercial
Definir estructura jurídica, tributaria y bancaria.

Abrir las cuentas empresariales necesarias y seleccionar proveedores de pago.

### Etapa 3 — Primeros ingresos
Activar cobros de forma controlada.

Registrar y medir todos los ingresos y costos reales.

### Etapa 4 — Internacionalización
Incorporar progresivamente monedas, métodos de pago y soluciones financieras adicionales según los mercados donde ZAREVOA consiga usuarios reales.

---

## 11. Principio de crecimiento

ZAREVOA no construirá una infraestructura financiera internacional compleja antes de necesitarla.

La estructura crecerá según:

- Número de usuarios.
- Volumen de ventas.
- Países de origen de los clientes.
- Monedas utilizadas.
- Costos de procesamiento.
- Necesidades operacionales reales.

El objetivo es mantener una operación financieramente ordenada desde el comienzo sin generar costos o complejidad innecesarios.

---

## Decisión ZAREVOA V1

Antes de activar cobros de ZAREVOA Journey, ZAREVOA Personal o ingresos relevantes provenientes de afiliados, deberá existir una estructura bancaria empresarial separada de las finanzas personales.

Como base se evaluará:

**Cuenta empresa CLP + cuenta empresa USD + capacidad internacional/SWIFT + posible solución multidivisa compatible con empresas chilenas.**

La implementación definitiva se realizará cuando ZAREVOA se aproxime a su etapa comercial.
