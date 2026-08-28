# 52 — Plan de métricas, KPIs y dashboard de ZAREVOA

## 1. Objetivo

Este documento define el sistema de métricas que permitirá evaluar el funcionamiento, crecimiento y sostenibilidad de ZAREVOA.

El objetivo no será acumular grandes cantidades de datos.

Será responder preguntas concretas:

- ¿Las personas encuentran valor en ZAREVOA?
- ¿El ZAREVOA Engine genera mejores viajes?
- ¿Los usuarios completan sus planificaciones?
- ¿Regresan?
- ¿Recomiendan el producto?
- ¿Están dispuestos a pagar?
- ¿El negocio puede crecer de manera sostenible?

Las métricas deberán ayudar a tomar decisiones.

---

## 2. Principio de medición

ZAREVOA deberá medir aquello que pueda generar una acción.

Una métrica sin capacidad de influir en una decisión tendrá prioridad secundaria.

La lógica será:

**Dato → Interpretación → Decisión → Acción → Resultado.**

---

## 3. Evitar medir por medir

La disponibilidad de herramientas analíticas puede generar cientos de métricas.

Esto no significa que todas sean importantes.

Durante la V1 deberá mantenerse un conjunto reducido de indicadores capaces de mostrar:

- adquisición;
- activación;
- calidad;
- conversión;
- retención;
- ingresos;
- costos;
- estabilidad.

---

## 4. Jerarquía de métricas

Las métricas podrán organizarse en cuatro niveles.

### Nivel 1 — Métrica principal

Representa el valor central entregado.

### Nivel 2 — KPIs estratégicos

Muestran salud general del producto y negocio.

### Nivel 3 — Métricas operativas

Ayudan a detectar problemas específicos.

### Nivel 4 — Diagnóstico

Permiten investigar las causas de un cambio.

Esto evitará que todos los números tengan la misma importancia.

---

## 5. North Star Metric

ZAREVOA deberá definir progresivamente una métrica principal vinculada al valor real generado.

Una candidata para la etapa inicial podría ser:

**Viajes útiles planificados con ZAREVOA.**

No bastará contar itinerarios generados automáticamente.

Idealmente deberá existir una señal de que el usuario encontró valor.

Por ejemplo:

- aprobó su ruta;
- realizó modificaciones;
- guardó el viaje;
- regresó al viaje;
- avanzó hacia preparación o reserva.

La definición definitiva deberá validarse con comportamiento real.

---

## 6. Viaje generado versus viaje útil

Esta distinción será fundamental.

**Viaje generado**

El sistema produjo un resultado.

**Viaje útil**

El usuario mostró señales de que ese resultado tenía valor.

ZAREVOA deberá optimizar principalmente el segundo.

---

## 7. Funnel principal

El funnel inicial podrá observar:

**Visita**

↓

**Inicio de planificación**

↓

**Travel Profile completado**

↓

**Tu ruta recomendada generada**

↓

**Ruta aprobada o modificada**

↓

**Itinerario generado**

↓

**Viaje guardado**

↓

**Usuario regresa**

↓

**Conversión o acción comercial**

Cada paso deberá poder medirse.

---

## 8. Adquisición

Las métricas de adquisición deberán mostrar de dónde llegan los usuarios.

Podrán incluir:

- visitas;
- usuarios nuevos;
- fuente;
- campaña;
- país;
- contenido;
- dispositivo;
- canal.

El volumen deberá analizarse junto con la calidad.

---

## 9. Calidad por canal

No todos los visitantes tendrán el mismo valor.

Por cada canal deberá observarse:

- inicio de planificación;
- Travel Profile completado;
- ruta generada;
- itinerario generado;
- conversión;
- retorno.

Un canal pequeño con usuarios altamente relevantes puede ser superior a uno con mucho tráfico y poca activación.

---

## 10. Activación

La activación deberá representar el momento en que un usuario experimenta por primera vez el valor principal de ZAREVOA.

Una posible definición inicial será:

> Usuario que completa Travel Profile y recibe una ruta recomendada coherente.

Esta definición podrá evolucionar según evidencia.

---

## 11. Tasa de activación

Podrá calcularse:

**Usuarios activados / usuarios que iniciaron planificación × 100**

Esta métrica permitirá detectar problemas en onboarding, formularios o generación.

---

## 12. Travel Profile

Deberán medirse aspectos como:

- porcentaje de inicio;
- porcentaje de finalización;
- tiempo de completado;
- campos abandonados;
- retrocesos;
- errores;
- modificaciones posteriores.

Esto permitirá simplificar el proceso sin perder información importante.

---

## 13. Abandono del formulario

Si muchos usuarios abandonan en una etapa específica deberá investigarse.

Posibles causas:

- pregunta poco clara;
- demasiadas opciones;
- formulario demasiado largo;
- información difícil de proporcionar;
- problema técnico;
- falta de percepción de valor.

No deberá eliminarse automáticamente una pregunta solo porque produzca abandono.

Primero deberá comprenderse su función.

---

## 14. Time to Value

Una métrica importante será:

**Tiempo hasta recibir valor.**

Podrá medirse desde que el usuario inicia planificación hasta que visualiza:

**Tu ruta recomendada.**

Reducir este tiempo puede mejorar activación siempre que no se reduzca la calidad.

---

## 15. Tu ruta recomendada

Esta pantalla deberá tener métricas propias.

Podrán medirse:

- aprobación directa;
- solicitud de alternativa;
- cambio de base;
- cambio de noches;
- eliminación de ciudad;
- incorporación de ciudad;
- abandono.

Esta información será especialmente valiosa para evaluar el Engine.

---

## 16. Tasa de aprobación de ruta

Una posible métrica será:

**Rutas aprobadas sin cambios / rutas mostradas.**

Sin embargo, no deberá interpretarse aisladamente.

Una modificación no significa necesariamente que el Engine haya fallado.

Puede reflejar personalización activa.

---

## 17. Tasa de modificación

También deberá observarse:

**Rutas modificadas / rutas mostradas.**

Las modificaciones podrán clasificarse.

Ejemplos:

- número de bases;
- orden;
- noches;
- Must See;
- presupuesto;
- ritmo;
- destino.

Los patrones repetitivos podrán revelar oportunidades de mejora.

---

## 18. Calidad del ZAREVOA Engine

La calidad no deberá medirse únicamente mediante una puntuación general.

Deberá observarse por dimensiones.

Por ejemplo:

- lógica geográfica;
- número de bases;
- tiempos de transición;
- ritmo;
- presupuesto;
- intereses;
- Must See;
- composición del grupo;
- coherencia diaria.

Esto permitirá identificar dónde falla realmente el sistema.

---

## 19. Evaluación explícita

Podrá solicitarse feedback simple después de determinados resultados.

Por ejemplo:

> ¿Esta ruta tiene sentido para tu viaje?

Opciones simples:

- Sí.
- Parcialmente.
- No.

Si la respuesta es negativa podrá solicitarse opcionalmente el motivo.

---

## 20. Evaluación implícita

El comportamiento también entrega señales.

Ejemplos:

- aceptar ruta;
- guardar;
- modificar;
- regenerar;
- regresar;
- eliminar viaje;
- abandonar inmediatamente.

Estas señales deberán combinarse con feedback explícito.

---

## 21. Regeneraciones

Un número alto de regeneraciones puede significar diferentes cosas.

Puede indicar:

- exploración;
- curiosidad;
- insatisfacción;
- falta de control;
- mala calidad.

Por ello deberá analizarse junto con otras acciones.

---

## 22. Itinerario detallado

Una vez generado el itinerario podrán medirse:

- visualización;
- tiempo de uso;
- días revisados;
- modificaciones;
- actividades eliminadas;
- actividades añadidas;
- cambios de ritmo;
- guardado.

Esto permitirá comprender qué partes aportan más valor.

---

## 23. Must See

Deberá comprobarse si los elementos marcados como Must See son correctamente incorporados.

Una métrica técnica posible será:

**Must See incorporados correctamente / Must See solicitados.**

Las excepciones deberán registrarse cuando exista imposibilidad real.

---

## 24. For You

Las recomendaciones For You podrán medirse mediante:

- visualización;
- aceptación;
- guardado;
- eliminación;
- sustitución;
- interacción.

El objetivo será aprender qué recomendaciones personalizadas realmente funcionan.

---

## 25. Presupuesto

El sistema deberá observar:

- presupuesto indicado;
- nivel seleccionado;
- estimación resultante;
- desviaciones;
- modificaciones posteriores.

Una recomendación atractiva pero incompatible con el presupuesto representa una falla de calidad.

---

## 26. Ritmo de viaje

Deberá analizarse si los usuarios mantienen o modifican:

- Relajado;
- Equilibrado;
- Intenso.

Si usuarios de un ritmo determinado eliminan sistemáticamente actividades, el Engine podría estar interpretando incorrectamente esa categoría.

---

## 27. Días de traslado

Los días con cambios de base deberán analizarse especialmente.

Podrán observarse:

- número de actividades;
- tiempo de transición;
- modificaciones;
- eliminación de actividades;
- feedback.

El objetivo será evitar itinerarios artificialmente sobrecargados.

---

## 28. Retención

La retención deberá responder:

> ¿Los usuarios vuelven a ZAREVOA después de experimentar el producto?

Podrá analizarse en ventanas como:

- día 1;
- día 7;
- día 30;
- antes del viaje;
- durante el viaje;
- después del viaje.

La frecuencia adecuada dependerá del ciclo natural de planificación.

---

## 29. Retención basada en viajes

Para ZAREVOA puede resultar más útil observar eventos del viaje que únicamente días calendario.

Ejemplos:

- vuelve después de crear ruta;
- vuelve antes de viajar;
- consulta durante el viaje;
- vuelve después;
- crea un segundo viaje.

Esto puede reflejar mejor el comportamiento real.

---

## 30. Segundo viaje

Una señal especialmente importante será:

**Usuarios que crean otro viaje.**

Esto puede indicar:

- confianza;
- utilidad;
- recuerdo de marca;
- intención de reutilización.

Con suficiente historial podrá convertirse en uno de los principales indicadores de fidelidad.

---

## 31. Conversión

Cuando existan productos de pago deberán medirse:

- usuarios expuestos a oferta;
- clics;
- inicio de compra;
- pago completado;
- abandono;
- reembolso.

Deberá distinguirse por producto.

---

## 32. Journey

Para ZAREVOA Journey podrán analizarse:

- tasa de conversión;
- precio;
- funciones utilizadas;
- satisfacción;
- costo;
- margen;
- repetición.

Esto permitirá comprobar si el producto premium realmente aporta valor adicional.

---

## 33. Personal

Para ZAREVOA Personal deberán añadirse métricas operativas.

Por ejemplo:

- clientes;
- solicitudes;
- tiempo humano;
- complejidad;
- satisfacción;
- costo por cliente;
- margen.

La demanda no deberá crecer por encima de la capacidad de atención.

---

## 34. Afiliación

Las métricas podrán incluir:

- visualizaciones de opciones reservables;
- clics;
- conversiones;
- valor de reservas;
- comisiones;
- cancelaciones;
- ingresos netos.

Deberán compararse por:

- proveedor;
- categoría;
- destino;
- mercado.

---

## 35. Recomendación versus monetización

Una métrica importante deberá comprobar que los incentivos comerciales no estén deteriorando la experiencia.

Podrá analizarse si las opciones afiliadas presentan diferencias significativas respecto de opciones no afiliadas en:

- aceptación;
- eliminación;
- satisfacción;
- reclamaciones.

La calidad deberá permanecer como criterio principal.

---

## 36. Ingresos

El dashboard financiero deberá mostrar progresivamente:

- ingresos totales;
- ingresos por Journey;
- ingresos por Personal;
- ingresos de afiliación;
- otros ingresos;
- reembolsos;
- ingresos netos.

Los ingresos deberán analizarse junto con costos.

---

## 37. Costos

Deberán medirse:

- infraestructura;
- IA;
- APIs;
- almacenamiento;
- pagos;
- herramientas;
- soporte;
- marketing;
- otros costos operativos.

Especialmente importante será conocer:

**Costo por viaje generado.**

---

## 38. Margen

Para cada producto deberá estimarse:

**Ingreso − costos variables directos = margen de contribución.**

Esto permitirá identificar qué productos pueden crecer de forma sostenible.

---

## 39. CAC

Cuando exista adquisición pagada deberá calcularse:

**CAC — Customer Acquisition Cost.**

Deberá poder observarse por:

- campaña;
- canal;
- país;
- producto;
- período.

No deberá escalarse publicidad sin comprender este indicador.

---

## 40. LTV

Con suficiente historial podrá estimarse:

**LTV — Lifetime Value.**

Deberá considerar:

- compras;
- viajes repetidos;
- afiliación;
- retención;
- productos adicionales.

Durante las primeras etapas será una estimación con alta incertidumbre.

---

## 41. LTV/CAC

La relación entre LTV y CAC ayudará a evaluar sostenibilidad de adquisición.

No deberá utilizarse como número absoluto durante etapas con pocos datos.

Será más importante observar su evolución.

---

## 42. Soporte

El dashboard deberá incluir métricas operativas como:

- solicitudes;
- categorías;
- primera respuesta;
- resolución;
- reapertura;
- satisfacción;
- problemas repetitivos.

Un aumento de soporte puede revelar problemas de producto.

---

## 43. Errores técnicos

Deberán medirse:

- errores;
- usuarios afectados;
- función;
- severidad;
- frecuencia;
- tiempo de resolución.

Los errores críticos deberán distinguirse claramente de problemas menores.

---

## 44. Disponibilidad

La plataforma deberá observar:

- disponibilidad;
- latencia;
- errores;
- fallos de proveedores;
- tiempos de generación.

No será necesario mostrar públicamente todas estas métricas durante la V1, pero deberán poder supervisarse internamente.

---

## 45. Rendimiento del Engine

Podrán medirse:

- tiempo de generación;
- costo de generación;
- fallos;
- reintentos;
- calidad;
- modificaciones posteriores.

El objetivo será mejorar simultáneamente:

**Calidad + velocidad + costo.**

---

## 46. Métricas de IA

Cuando la IA intervenga deberán observarse aspectos como:

- consumo;
- costo;
- latencia;
- errores;
- respuestas inválidas;
- necesidad de regeneración.

Esto permitirá decidir qué tareas necesitan IA y cuáles pueden resolverse mediante reglas o datos estructurados.

---

## 47. Segmentación

Las métricas podrán segmentarse cuando exista volumen suficiente.

Ejemplos:

- país;
- idioma;
- dispositivo;
- duración del viaje;
- presupuesto;
- ritmo;
- tipo de grupo;
- destino;
- usuario nuevo o recurrente.

La segmentación deberá tener una finalidad concreta.

---

## 48. Cohortes

El análisis por cohortes permitirá comparar grupos de usuarios que comenzaron en períodos similares.

Por ejemplo:

- usuarios registrados en una semana;
- usuarios adquiridos mediante una campaña;
- usuarios de un país;
- usuarios que utilizaron determinada versión.

Esto ayudará a distinguir mejoras reales de cambios en composición del tráfico.

---

## 49. Experimentos

Cada experimento deberá definir antes de comenzar:

- hipótesis;
- métrica principal;
- métricas secundarias;
- posible riesgo;
- período;
- criterio de éxito.

No deberá modificarse la definición de éxito después de observar los resultados.

---

## 50. Métricas de protección

Una mejora en una métrica no deberá perjudicar otras áreas importantes.

Por ello podrán utilizarse métricas de protección.

Ejemplo:

Una modificación aumenta conversión.

Pero también aumenta:

- reembolsos;
- reclamaciones;
- abandono posterior.

Entonces el resultado puede no ser positivo.

---

## 51. Vanity Metrics

ZAREVOA deberá evitar decisiones basadas únicamente en métricas de apariencia.

Ejemplos:

- impresiones;
- seguidores;
- visitas sin intención;
- itinerarios generados automáticamente;
- descargas sin uso.

Estas métricas pueden aportar contexto, pero no deberán confundirse con valor.

---

## 52. Dashboard ejecutivo

El dashboard principal deberá ser simple.

Podrá incluir inicialmente:

### Producto

- usuarios activos;
- planificaciones iniciadas;
- Travel Profiles completados;
- rutas recomendadas;
- itinerarios completados.

### Calidad

- aprobación de ruta;
- modificaciones;
- feedback;
- problemas del Engine.

### Negocio

- conversiones;
- ingresos;
- costos;
- margen.

### Operación

- errores;
- soporte;
- disponibilidad.

El objetivo será poder comprender rápidamente el estado general de ZAREVOA.

---

## 53. Dashboard del Engine

Deberá existir progresivamente una vista específica para el ZAREVOA Engine.

Podrá mostrar:

- rutas generadas;
- aprobación;
- cambios de bases;
- cambios de noches;
- regeneraciones;
- errores;
- satisfacción;
- costo;
- latencia.

Esta información será fundamental para mejorar el criterio propio de ZAREVOA.

---

## 54. Dashboard financiero

Deberá mostrar:

- ingresos;
- costos;
- margen;
- pagos;
- reembolsos;
- afiliación;
- CAC;
- gasto publicitario;
- flujo de caja cuando corresponda.

La complejidad deberá crecer con el negocio.

---

## 55. Dashboard de soporte

Podrá mostrar:

- solicitudes abiertas;
- prioridad;
- categoría;
- tiempo de respuesta;
- tiempo de resolución;
- satisfacción;
- problemas recurrentes.

También deberá identificar posibles incidentes.

---

## 56. Frecuencia de revisión

Durante la V1 podrá utilizarse:

### Diario

- errores críticos;
- disponibilidad;
- pagos;
- incidencias.

### Semanal

- producto;
- Engine;
- soporte;
- adquisición;
- feedback.

### Mensual

- crecimiento;
- conversión;
- ingresos;
- costos;
- retención;
- estrategia.

No todas las métricas necesitan revisarse diariamente.

---

## 57. Alertas

Algunas métricas deberán generar alertas automáticas cuando superen determinados límites.

Ejemplos:

- aumento brusco de errores;
- caída de generación;
- problemas de pagos;
- aumento de latencia;
- proveedor externo caído;
- costo anormal de IA.

Los umbrales deberán ajustarse con experiencia real.

---

## 58. Privacidad y analítica

La medición deberá respetar los principios de privacidad definidos por ZAREVOA.

Deberá evitarse recopilar información únicamente porque técnicamente sea posible.

Los datos deberán tener una finalidad clara.

Cuando corresponda deberán aplicarse:

- consentimiento;
- minimización;
- anonimización;
- retención limitada;
- controles de acceso.

---

## 59. Fuente única de verdad

Las métricas importantes deberán tener definiciones documentadas.

Por ejemplo:

**Usuario activo**

**Viaje generado**

**Ruta aprobada**

**Conversión**

**Usuario de pago**

Esto evitará que diferentes dashboards calculen el mismo indicador de maneras distintas.

---

## 60. Diccionario de métricas

Deberá mantenerse progresivamente un registro con:

- nombre;
- definición;
- fórmula;
- fuente;
- frecuencia;
- responsable;
- interpretación.

Este documento podrá crecer junto con la plataforma.

---

## 61. Datos históricos

Los cambios en definiciones deberán registrarse.

Si una métrica cambia de fórmula, deberá ser posible comprender desde qué fecha ocurrió.

Esto evitará comparaciones incorrectas entre períodos.

---

## 62. Prioridades de la V1

Durante la primera versión no será necesario implementar todos los indicadores descritos.

La prioridad será conocer:

1. cuántas personas comienzan un viaje;
2. cuántas completan Travel Profile;
3. cuántas reciben su ruta;
4. cuántas la aceptan o modifican;
5. cuántas completan el itinerario;
6. cuántas regresan;
7. qué problemas encuentran;
8. cuánto cuesta generar cada viaje.

Cuando exista monetización:

9. cuántas pagan;
10. cuánto ingreso y margen generan.

---

## 63. Decisiones basadas en evidencia

Las métricas deberán complementar el criterio de producto.

No deberán sustituirlo completamente.

Una cifra puede indicar:

**qué está ocurriendo.**

El análisis cualitativo puede ayudar a explicar:

**por qué está ocurriendo.**

ZAREVOA deberá utilizar ambos.

---

## 64. Ciclo de aprendizaje

El sistema de medición deberá alimentar un ciclo continuo:

**Medir**

↓

**Detectar**

↓

**Investigar**

↓

**Priorizar**

↓

**Modificar**

↓

**Volver a medir**

Este ciclo será una de las bases de evolución de ZAREVOA.

---

## 65. Resultado esperado

Un buen sistema de métricas permitirá responder rápidamente:

- si ZAREVOA está creciendo;
- si está mejorando;
- si el Engine funciona;
- si los usuarios encuentran valor;
- si existen problemas;
- si la monetización funciona;
- si los costos son sostenibles.

Las decisiones dejarán de depender únicamente de intuición.

---

## 66. Principio final

El éxito de ZAREVOA no deberá medirse por cuántos itinerarios puede producir una máquina.

Deberá medirse por cuántas personas reciben una planificación que realmente les ayuda a viajar mejor.

Por ello, el indicador más importante siempre deberá permanecer conectado al valor real entregado al viajero.

---

## 67. Cierre

Las métricas serán el sistema de observación de ZAREVOA.

El ZAREVOA Engine aportará criterio.

Los usuarios aportarán comportamiento y feedback.

Los datos permitirán comprobar qué funciona.

La combinación será:

**Criterio + Usuarios + Datos + Aprendizaje continuo.**

El objetivo no será construir el dashboard con más números.

Será construir el sistema que permita tomar mejores decisiones.

**ZAREVOA — PLAN YOUR WORLD**
