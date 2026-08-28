# ZAREVOA — Plan de Internacionalización, Idiomas, Monedas y Mercados

## 1. Objetivo

Este documento define la estrategia inicial para convertir ZAREVOA progresivamente en una plataforma internacional.

La internacionalización no deberá consistir únicamente en traducir la interfaz.

Deberá permitir que una persona pueda utilizar ZAREVOA desde distintos países y recibir una experiencia adaptada a su contexto en aspectos como:

- Idioma.
- Moneda.
- Formato de fechas.
- Formato de horas.
- Unidades.
- Presupuesto.
- Métodos de pago.
- Información de viaje.
- Proveedores.
- Regulaciones.
- Comunicación.

El principio será:

**ZAREVOA deberá sentirse local para el usuario sin dejar de ser una marca global.**

---

# A. VISIÓN INTERNACIONAL

## 2. Marca global

ZAREVOA nace con vocación internacional.

La marca principal será:

**ZAREVOA**

y deberá mantenerse consistente entre mercados.

---

## 3. Tagline

El tagline:

**PLAN YOUR WORLD**

podrá mantenerse como elemento internacional de identidad.

---

## 4. Expansión progresiva

Tener vocación global no significa intentar operar completamente en todos los países desde V1.

La expansión deberá ser:

**controlada + medible + basada en calidad.**

---

# B. INTERNACIONALIZACIÓN VS LOCALIZACIÓN

## 5. Internacionalización

Consiste en construir la plataforma técnicamente preparada para diferentes:

- Idiomas.
- Monedas.
- Regiones.
- Formatos.
- Mercados.

---

## 6. Localización

Consiste en adaptar la experiencia a un mercado específico.

Puede incluir:

- Traducción.
- Terminología.
- Moneda.
- Formato.
- Mensajes.
- Proveedores.
- Métodos de pago.
- Consideraciones culturales.

---

## 7. Principio

**Traducir no es localizar.**

---

# C. ARQUITECTURA INTERNACIONAL DESDE V1

## 8. Preparación técnica

Aunque inicialmente exista un número reducido de idiomas, el sistema deberá evitar decisiones que dificulten añadir otros posteriormente.

---

## 9. Textos de interfaz

Los textos visibles no deberían quedar dispersos directamente dentro del código cuando pueda evitarse.

Deberán poder gestionarse mediante una estructura preparada para internacionalización.

---

## 10. Contenido dinámico

Deberá diferenciarse entre:

- Texto de interfaz.
- Contenido editorial.
- Contenido de proveedores.
- Datos estructurados.
- Contenido generado por IA.

Cada categoría puede requerir una estrategia diferente de traducción.

---

# D. IDIOMAS INICIALES

## 11. Español

El español podrá funcionar como uno de los idiomas iniciales principales de ZAREVOA.

---

## 12. Inglés

El inglés deberá considerarse prioritario para la expansión internacional.

---

## 13. Arquitectura

Desde V1 convendrá utilizar códigos estándar de idioma/región.

Ejemplos:

- `es`
- `en`

Y posteriormente, cuando sea necesario:

- `es-CL`
- `es-ES`
- `en-US`
- `en-GB`
- `en-CA`

---

# E. NUEVOS IDIOMAS

## 14. No añadir por intuición

Un nuevo idioma deberá incorporarse cuando existan señales suficientes.

---

## 15. Criterios

Evaluar:

- Tráfico.
- Demanda.
- Usuarios.
- Destinos.
- Conversión.
- Monetización.
- Costos.
- Competencia.
- Capacidad de soporte.

---

## 16. Posibles idiomas futuros

Dependiendo de la demanda real podrán evaluarse:

- Portugués.
- Francés.
- Alemán.
- Italiano.
- Japonés.
- Coreano.
- Chino.

La lista no representa un compromiso ni orden definitivo.

---

# F. CALIDAD DE TRADUCCIÓN

## 17. Objetivo

Una traducción deberá sonar natural para un viajero.

No como una traducción automática literal.

---

## 18. Especial atención

Revisar cuidadosamente:

- CTAs.
- Travel Profile.
- Presupuesto.
- Ritmos.
- Mensajes de error.
- Pagos.
- Privacidad.
- Journey.
- Personal.

---

# G. IA Y TRADUCCIÓN

## 19. Uso

La IA podrá ayudar a:

- Traducir.
- Adaptar.
- Revisar consistencia.
- Generar variantes.

---

## 20. Control

Los textos importantes deberán tener mecanismos de revisión.

Especialmente:

- Legales.
- Comerciales.
- Seguridad.
- Pagos.
- Información crítica de viaje.

---

# H. GLOSARIO ZAREVOA

## 21. Necesidad

Deberá mantenerse un glosario oficial para términos propios.

Ejemplos:

- Travel Profile.
- Must See.
- For You.
- Tu ruta recomendada.
- Journey.
- Personal.
- ZAREVOA Engine.

---

## 22. Objetivo

Evitar que una misma función tenga diferentes nombres según la pantalla o traducción.

---

# I. TRADUCCIÓN DE MARCA

## 23. Elementos que normalmente no se traducen

Mantener:

**ZAREVOA**

**ZAREVOA Journey**

**ZAREVOA Personal**

---

## 24. Tagline

**PLAN YOUR WORLD**

podrá mantenerse globalmente mientras sea coherente con la estrategia de marca.

---

# J. IDIOMA DEL USUARIO

## 25. Detección

La plataforma podrá detectar inicialmente el idioma del navegador o dispositivo.

---

## 26. Control

El usuario deberá poder cambiarlo manualmente.

---

## 27. Preferencia

Cuando el usuario seleccione un idioma deberá guardarse como preferencia cuando corresponda.

---

# K. IDIOMA DEL VIAJE

## 28. Diferenciación

El idioma de la interfaz y el idioma del destino no son lo mismo.

Ejemplo:

Un usuario chileno puede utilizar ZAREVOA en español para viajar a Japón.

---

## 29. Resultado

La información deberá presentarse en el idioma del usuario cuando sea posible, manteniendo nombres locales cuando sean útiles.

---

# L. NOMBRES DE LUGARES

## 30. Principio

Los lugares podrán requerir:

- Nombre localizado.
- Nombre oficial.
- Nombre local.

---

## 31. Ejemplo conceptual

Mostrar un nombre comprensible para el viajero sin dificultar que pueda reconocerlo en mapas, estaciones o señalización local.

---

# M. CARACTERES INTERNACIONALES

## 32. Compatibilidad

ZAREVOA deberá soportar correctamente caracteres Unicode.

Esto incluye:

- Tildes.
- Ñ.
- Alfabetos no latinos.
- Nombres internacionales.

---

## 33. Datos

No deberán modificarse nombres propios únicamente porque el sistema no soporte determinados caracteres.

---

# N. MONEDAS

## 34. Objetivo

El usuario deberá poder comprender costos en una moneda relevante para él.

---

## 35. Monedas iniciales

Dependiendo del mercado inicial podrán considerarse:

- CLP.
- USD.
- EUR.

Posteriormente podrán añadirse otras.

---

## 36. Escalabilidad

La arquitectura deberá permitir monedas adicionales sin modificar toda la lógica financiera.

---

# O. MONEDA DE ORIGEN VS DESTINO

## 37. Diferencia

Un usuario puede:

- Vivir en Chile.
- Tener presupuesto en CLP.
- Viajar a Italia.
- Comprar servicios en EUR.

---

## 38. ZAREVOA

Deberá diferenciar cuando corresponda:

- Moneda del usuario.
- Moneda del presupuesto.
- Moneda local.
- Moneda del proveedor.

---

# P. CONVERSIÓN DE MONEDA

## 39. Tipo de cambio

Cuando se utilicen conversiones deberán provenir de una fuente adecuada y actualizarse con una frecuencia razonable.

---

## 40. Transparencia

Los valores convertidos deberán considerarse:

**estimaciones.**

---

## 41. Evitar falsa precisión

No presentar una conversión como precio final garantizado si el proveedor procesa el pago en otra moneda.

---

# Q. FORMATO DE MONEDA

## 42. Localización

El formato deberá adaptarse cuando corresponda.

Ejemplos:

- $100.000 CLP
- US$100
- €100

---

## 43. Ambigüedad

Cuando el símbolo `$` pueda generar confusión deberá mostrarse el código de moneda.

---

# R. PRESUPUESTO INTERNACIONAL

## 44. Niveles ZAREVOA

Mantener conceptualmente:

- Económico.
- Equilibrado.
- Confort.
- Premium.

---

## 45. No usar cifras universales

Un presupuesto considerado Premium en un destino puede ser insuficiente en otro.

---

## 46. Contexto

Los niveles deberán adaptarse según:

- Destino.
- Temporada.
- Duración.
- Grupo.
- Moneda.
- Costos reales disponibles.

---

# S. PRESUPUESTO DEFINIDO

## 47. Usuario

El usuario podrá indicar un presupuesto concreto.

---

## 48. Engine

El ZAREVOA Engine deberá trabajar internamente con una representación consistente del presupuesto.

---

## 49. Conversión

Cuando sea necesario, convertir valores para compararlos sin perder información sobre la moneda original.

---

# T. FECHAS

## 50. Diferencias regionales

Ejemplos:

- `27/08/2026`
- `08/27/2026`

---

## 51. Interfaz

La presentación deberá adaptarse a la configuración regional.

---

## 52. Datos internos

Internamente deberán utilizarse formatos estándar que eviten ambigüedad.

---

# U. HORA

## 53. Formatos

Los usuarios pueden preferir:

- 24 horas.
- AM/PM.

---

## 54. Zonas horarias

Los viajes internacionales pueden cruzar varias zonas horarias.

El sistema deberá evitar asumir que:

**hora del usuario = hora del destino.**

---

## 55. Datos

Cuando sea relevante, almacenar o calcular utilizando información explícita de zona horaria.

---

# V. CAMBIOS DE FECHA

## 56. Viajes internacionales

Un vuelo puede salir un día y llegar otro debido a:

- Duración.
- Zona horaria.
- Línea internacional de cambio de fecha.

---

## 57. Engine

El cálculo de días deberá respetar esta realidad.

---

# W. UNIDADES

## 58. Distancias

Dependiendo del mercado:

- Kilómetros.
- Millas.

---

## 59. Temperatura

Dependiendo del usuario:

- Celsius.
- Fahrenheit.

---

## 60. Preferencias

Cuando sea razonable, permitir configurar o inferir las unidades.

---

# X. DIRECCIONES

## 61. Formatos

Los formatos de dirección varían entre países.

La base de datos no deberá diseñarse asumiendo una única estructura universal.

---

# Y. TELÉFONOS

## 62. Internacionalización

Cuando se almacenen números telefónicos deberán considerarse:

- Código de país.
- Formato internacional.
- Validación.

---

# Z. MERCADOS

## 63. Definición

Un mercado no será simplemente:

**un país donde alguien puede abrir la web.**

Para efectos estratégicos, un mercado deberá analizarse según la capacidad de ZAREVOA de ofrecer una experiencia suficientemente buena y sostenible.

---

# AA. CRITERIOS PARA ABRIR UN MERCADO

## 64. Demanda

Analizar:

- Búsquedas.
- Usuarios.
- Tráfico.
- Intención de viaje.

---

## 65. Producto

Verificar:

- Idioma.
- Calidad del Engine.
- Cobertura de destinos.
- Datos.
- UX.

---

## 66. Comercial

Verificar:

- Pagos.
- Moneda.
- Afiliados.
- Potencial de ingresos.

---

## 67. Operacional

Verificar:

- Soporte.
- Proveedores.
- Costos.
- Monitoreo.

---

## 68. Legal

Verificar:

- Privacidad.
- Consumidor.
- Cookies.
- Pagos.
- Marketing.
- Obligaciones locales.

---

# AB. MATRIZ DE EVALUACIÓN DE MERCADO

## 69. Variables

Cada mercado podrá evaluarse del 1 al 5 en:

- Demanda.
- Calidad de datos.
- Facilidad de localización.
- Potencial comercial.
- Competencia.
- Complejidad legal.
- Costos.
- Capacidad de soporte.

---

## 70. Decisión

La puntuación no deberá sustituir el criterio.

Servirá para comparar oportunidades.

---

# AC. PAÍS DEL USUARIO VS DESTINO

## 71. Dos dimensiones

ZAREVOA deberá diferenciar:

**mercado de origen**

y

**mercado de destino.**

---

## 72. Ejemplo

Un usuario en Chile que viaja a Francia representa:

- Mercado de origen: Chile.
- Destino: Francia.

Ambos afectan diferentes partes del producto.

---

# AD. COBERTURA DE DESTINOS

## 73. Calidad antes que cantidad

No será necesario afirmar que ZAREVOA conoce perfectamente todo el planeta desde el primer día.

---

## 74. Estrategia

Podrá comenzar con mejor cobertura en destinos donde existan:

- Datos fiables.
- Demanda.
- Buenas conexiones.
- Información suficiente.

---

# AE. NIVELES DE COBERTURA

## 75. Concepto

Los destinos podrán clasificarse internamente.

### Nivel A

Cobertura alta.

### Nivel B

Cobertura adecuada.

### Nivel C

Cobertura limitada.

---

## 76. Uso

Esta clasificación podrá ayudar al Engine a conocer cuándo existe suficiente información para realizar determinadas recomendaciones.

---

# AF. NO OCULTAR LIMITACIONES

## 77. Transparencia

Si ZAREVOA tiene información limitada sobre una región deberá evitar presentar el mismo nivel de certeza que en destinos con cobertura alta.

---

# AG. DATOS INTERNACIONALES

## 78. Fuentes

Los proveedores deberán evaluarse por:

- Cobertura geográfica.
- Precisión.
- Actualización.
- Licencia.
- Precio.
- Idiomas.
- Límites.
- Estabilidad.

---

## 79. Evitar dependencia única

Cuando una fuente sea crítica deberá evaluarse el riesgo de depender exclusivamente de ella.

---

# AH. MAPAS

## 80. Internacionalización

La solución de mapas deberá funcionar correctamente en los mercados objetivo.

---

## 81. Evaluación

Considerar:

- Cobertura.
- Rutas.
- Transporte.
- Geocodificación.
- Costos.
- Restricciones regionales.

---

# AI. TRANSPORTE

## 82. Complejidad

La disponibilidad de información varía según país.

Puede incluir:

- Tren.
- Metro.
- Bus.
- Ferry.
- Vuelo.
- Automóvil.

---

## 83. Engine

No deberá asumir que todos los destinos tienen las mismas alternativas.

---

# AJ. HORARIOS

## 84. Información dinámica

Horarios de:

- Atracciones.
- Transporte.
- Restaurantes.
- Servicios.

pueden cambiar.

---

## 85. Presentación

Cuando sea necesario deberá indicarse que determinada información debe verificarse antes del viaje.

---

# AK. PROVEEDORES COMERCIALES

## 86. Variación regional

Un proveedor de reservas puede funcionar muy bien en Europa y tener cobertura limitada en otro mercado.

---

## 87. Estrategia

ZAREVOA podrá utilizar distintos partners según:

- Destino.
- Mercado.
- Producto.
- Conversión.

---

# AL. AFILIADOS INTERNACIONALES

## 88. Evaluar

Antes de activar un programa revisar:

- Países permitidos.
- Monedas.
- Pagos de comisión.
- Métodos de cobro.
- Condiciones.
- Tracking.
- Impuestos.
- Conversión.

---

# AM. PAGOS INTERNACIONALES

## 89. Objetivo

Cuando ZAREVOA cobre directamente deberá permitir una experiencia sencilla para los mercados habilitados.

---

## 90. Proveedor

Evaluar:

- Países soportados.
- Monedas.
- Métodos de pago.
- Fees.
- Conversión.
- Chargebacks.
- Reembolsos.
- Integración.

---

# AN. ESTRUCTURA BANCARIA

## 91. Separación

Antes de activar cobros comerciales deberá existir separación adecuada entre finanzas personales y empresariales.

---

## 92. Necesidades iniciales

Evaluar:

- Cuenta empresa en CLP.
- Cuenta empresa en USD.
- Transferencias internacionales.
- SWIFT.
- Solución multidivisa compatible cuando sea conveniente.

---

## 93. Objetivo

Facilitar:

- Cobros.
- Comisiones.
- Proveedores.
- Reconciliación.
- Contabilidad.
- Expansión internacional.

---

# AO. IMPUESTOS

## 94. Variación

Los impuestos sobre servicios digitales pueden depender de:

- País del negocio.
- País del cliente.
- Tipo de servicio.
- Volumen.
- Estructura jurídica.

---

## 95. Revisión profesional

Antes de escalar ventas internacionales deberá realizarse revisión contable y tributaria profesional.

---

# AP. PRIVACIDAD INTERNACIONAL

## 96. Principio

Una plataforma global puede quedar sujeta a diferentes marcos de privacidad.

---

## 97. Estrategia

Mantener desde el diseño:

- Minimización.
- Transparencia.
- Seguridad.
- Control del usuario.
- Registro de proveedores.

---

## 98. Expansión

Antes de abrir mercados importantes deberá revisarse la regulación aplicable.

---

# AQ. TÉRMINOS Y POLÍTICAS

## 99. Localización legal

No asumir que traducir los términos de un país automáticamente los hace válidos en otro.

---

## 100. Revisión

Los mercados importantes podrán requerir adaptación jurídica.

---

# AR. COOKIES

## 101. Diferencias

Los requisitos de consentimiento pueden variar por jurisdicción.

---

## 102. Diseño

La arquitectura de consentimiento deberá poder adaptarse.

---

# AS. MARKETING INTERNACIONAL

## 103. Mensaje central

Mantener la esencia:

**planificación personalizada + realismo + control.**

---

## 104. Adaptación

El lenguaje comercial podrá variar según cultura y mercado.

---

# AT. SEO INTERNACIONAL

## 105. Arquitectura

Cuando existan varios idiomas deberá utilizarse una estructura SEO clara.

---

## 106. Contenido

No traducir automáticamente miles de páginas sin revisar calidad e intención de búsqueda.

---

## 107. Búsquedas locales

Las personas pueden buscar de forma diferente aunque estén buscando el mismo tipo de viaje.

---

# AU. DOMINIO

## 108. Marca

La estrategia deberá favorecer una identidad global centralizada.

---

## 109. Idiomas

Cuando sea adecuado podrán utilizarse rutas como:

- `/es/`
- `/en/`

en lugar de crear infraestructuras completamente separadas para cada mercado.

---

# AV. SOPORTE INTERNACIONAL

## 110. Idiomas de soporte

No ofrecer oficialmente soporte en un idioma que ZAREVOA no pueda gestionar adecuadamente.

---

## 111. IA

La IA podrá ayudar con traducción de soporte, pero los casos complejos deberán mantener control suficiente.

---

# AW. HORARIOS DE SOPORTE

## 112. Zonas horarias

Una base internacional implica consultas en diferentes horarios.

---

## 113. V1

No prometer soporte 24/7 si no existe capacidad real.

---

## 114. Evolución

La cobertura podrá ampliarse cuando:

- Volumen.
- Ingresos.
- Journey.
- Personal.

lo justifiquen.

---

# AX. JOURNEY INTERNACIONAL

## 115. Importancia

Journey aumentará la necesidad de:

- Horarios correctos.
- Zona horaria.
- Información local.
- Transporte.
- Moneda.
- Idioma.
- Datos actualizados.

---

## 116. Urgencia

La información utilizada durante un viaje puede ser más sensible al tiempo que la utilizada meses antes.

---

# AY. PERSONAL INTERNACIONAL

## 117. Expansión

Antes de ofrecer Personal ampliamente deberán definirse:

- Idiomas.
- Horarios.
- Capacidad.
- Mercados.
- Alcance.

---

# AZ. EMERGENCIAS

## 118. Límites

ZAREVOA no deberá presentarse como servicio internacional de emergencias.

---

## 119. Información

Cuando corresponda podrá orientar hacia fuentes oficiales, manteniendo claridad sobre su función.

---

# BA. DOCUMENTACIÓN DE VIAJE

## 120. Futuro

ZAREVOA podrá ayudar a organizar información sobre:

- Pasaporte.
- Visas.
- Requisitos.
- Seguro.
- Documentos.

---

## 121. Riesgo

Estos requisitos pueden cambiar y tener consecuencias importantes.

La información deberá apoyarse en fuentes adecuadas y recomendar verificación oficial.

---

# BB. VISAS Y FRONTERAS

## 122. No generalizar

Los requisitos dependen de:

- Nacionalidad.
- Destino.
- Escalas.
- Duración.
- Motivo.

---

## 123. Diseño

Nunca inferir automáticamente que una regla migratoria aplica a todos los usuarios.

---

# BC. SEGURIDAD DEL VIAJERO

## 124. Fuentes

Cuando se incorpore información de seguridad deberá priorizarse información oficial y actualizada.

---

## 125. Neutralidad

Evitar alarmismo o falsa tranquilidad.

---

# BD. ACCESIBILIDAD INTERNACIONAL

## 126. Diseño

La expansión deberá considerar:

- Tamaño de texto.
- Lectores de pantalla.
- Contraste.
- Navegación.
- Diferencias de longitud entre idiomas.

---

# BE. RTL

## 127. Futuro

Si se incorporan idiomas escritos de derecha a izquierda, la interfaz deberá estar técnicamente preparada para adaptarse.

---

# BF. DISEÑO Y LONGITUD

## 128. Problema

Una frase puede ocupar mucho más espacio en un idioma que en otro.

---

## 129. Regla

Los componentes no deberán depender de textos con longitud fija.

---

# BG. BÚSQUEDA

## 130. Internacionalización

La búsqueda deberá tolerar:

- Tildes.
- Variantes.
- Nombres locales.
- Nombres traducidos.
- Diferentes alfabetos.

---

# BH. SLUGS Y URLs

## 131. Diseño

Las URLs deberán mantenerse:

- Claras.
- Estables.
- Compatibles con internacionalización.

---

# BI. EMAILS

## 132. Localización

Los correos deberán respetar:

- Idioma.
- Zona horaria cuando corresponda.
- Moneda.
- Contexto del viaje.

---

# BJ. NOTIFICACIONES

## 133. Hora local

Una notificación relacionada con el viaje deberá considerar la zona horaria adecuada.

---

## 134. Evitar

No enviar recordatorios de viaje a horas absurdas por utilizar únicamente la zona horaria del servidor.

---

# BK. ANALYTICS

## 135. Segmentación

Medir por:

- País.
- Idioma.
- Moneda.
- Mercado de origen.
- Destino.

---

## 136. Privacidad

La medición deberá mantener los principios de minimización y cumplimiento aplicables.

---

# BL. MÉTRICAS POR MERCADO

## 137. Evaluar

- Usuarios.
- Activación.
- Viajes útiles.
- Retención.
- Conversión.
- Ingresos.
- CAC.
- Costos.
- Soporte.

---

# BM. MÉTRICAS POR IDIOMA

## 138. Comparar

Un idioma puede tener:

- Mucho tráfico.
- Baja activación.

Esto puede indicar:

- Traducción deficiente.
- Mercado diferente.
- Problema de UX.
- Expectativas distintas.

---

# BN. CALIDAD POR DESTINO

## 139. Medición

No medir únicamente calidad global.

Analizar también:

- País.
- Ciudad.
- Tipo de viaje.
- Duración.

---

## 140. Objetivo

Detectar dónde el Engine funciona especialmente bien o mal.

---

# BO. PRUEBAS INTERNACIONALES

## 141. Casos

Antes de habilitar un nuevo mercado probar:

- Idioma.
- Moneda.
- Fechas.
- Horas.
- Direcciones.
- Pagos.
- Emails.
- Travel Profile.
- Engine.
- Ruta.
- Itinerario.

---

# BP. MATRIZ DE PRUEBAS

## 142. Ejemplos

Probar combinaciones como:

**Usuario Chile → Viaje España**

**Usuario Canadá → Viaje Japón**

**Usuario EE. UU. → Viaje Italia**

**Usuario España → Viaje Chile**

---

## 143. Objetivo

Detectar supuestos regionales ocultos dentro del producto.

---

# BQ. LANZAMIENTO DE NUEVO MERCADO

## 144. Fase 1

Investigación.

---

## 145. Fase 2

Preparación técnica.

---

## 146. Fase 3

Localización.

---

## 147. Fase 4

Pruebas.

---

## 148. Fase 5

Beta limitada.

---

## 149. Fase 6

Lanzamiento controlado.

---

## 150. Fase 7

Medición.

---

# BR. CRITERIOS GO/NO-GO

## 151. GO

Un mercado podrá abrirse cuando exista:

- Producto funcional.
- Calidad suficiente.
- Datos adecuados.
- Idioma correcto.
- Operación posible.
- Cumplimiento revisado.
- Capacidad de medir.

---

## 152. NO-GO

Posponer si:

- Engine funciona mal.
- Datos son insuficientes.
- Traducción es deficiente.
- Pagos no funcionan.
- Riesgo legal es desconocido.
- Soporte no puede atenderlo.

---

# BS. PRIORIZACIÓN DE MERCADOS

## 153. No utilizar únicamente tamaño

Un mercado enorme puede ser difícil y costoso.

Un mercado más pequeño puede ofrecer mejor oportunidad inicial.

---

## 154. Fórmula conceptual

Evaluar:

**Demanda × Ajuste de producto × Potencial comercial**

frente a:

**Costo × Complejidad × Riesgo**

---

# BT. EXPANSIÓN POR ETAPAS

## 155. Etapa inicial

Concentrarse en:

- Idiomas prioritarios.
- Destinos de buena cobertura.
- Experiencia sólida.

---

## 156. Segunda etapa

Añadir:

- Más destinos.
- Monedas.
- Proveedores.
- Mercados.

---

## 157. Tercera etapa

Profundizar localización y monetización.

---

## 158. Largo plazo

Convertir ZAREVOA en una plataforma global con capacidad de adaptación regional.

---

# BU. EVITAR SOBREEXPANSIÓN

## 159. Riesgo

Expandirse demasiado rápido puede producir:

- Mala traducción.
- Información insuficiente.
- Soporte complejo.
- Costos.
- Problemas legales.
- Experiencia inconsistente.

---

## 160. Principio

**Cobertura global superficial no será mejor que cobertura selectiva de alta calidad.**

---

# BV. ESCALABILIDAD TÉCNICA

## 161. Preparar

La arquitectura deberá evitar que añadir un nuevo idioma o moneda requiera reconstruir la plataforma.

---

## 162. Configuración

Siempre que sea posible utilizar:

- Configuración.
- Catálogos.
- Feature flags.
- Servicios independientes.

---

# BW. FEATURE FLAGS

## 163. Uso

Permitir activar funciones según:

- País.
- Idioma.
- Mercado.
- Usuario.

---

## 164. Beneficio

Facilita pruebas y expansión controlada.

---

# BX. FALLBACKS

## 165. Idioma

Si falta una traducción deberá existir una estrategia de fallback.

---

## 166. Datos

Si un proveedor no tiene cobertura suficiente deberá existir comportamiento definido.

---

## 167. Moneda

Si una moneda no está disponible deberá evitarse mostrar conversiones inventadas.

---

# BY. COSTOS INTERNACIONALES

## 168. Registrar

La expansión puede aumentar:

- IA.
- APIs.
- Traducción.
- Soporte.
- Pagos.
- Legal.
- Marketing.

---

## 169. Evaluación

Cada mercado deberá analizarse también desde sostenibilidad económica.

---

# BZ. MERCADO RENTABLE VS MERCADO POPULAR

## 170. Diferencia

El mercado con más usuarios no necesariamente será el mercado más rentable.

---

## 171. Analizar

Comparar:

- Activación.
- Retención.
- CAC.
- Monetización.
- Costos operativos.

---

# CA. APRENDIZAJE

## 172. Expansión como experimento

Cada nuevo mercado deberá producir conocimiento.

---

## 173. Documentar

Registrar:

- Hipótesis.
- Resultados.
- Problemas.
- Costos.
- Conversiones.
- Decisiones.

---

# CB. CHECKLIST DE NUEVO IDIOMA

## 174. Antes de activar

- [ ] Interfaz traducida.
- [ ] Travel Profile revisado.
- [ ] Ruta revisada.
- [ ] Itinerario revisado.
- [ ] Emails revisados.
- [ ] Errores revisados.
- [ ] Glosario consistente.
- [ ] Formatos locales correctos.
- [ ] QA completado.

---

# CC. CHECKLIST DE NUEVA MONEDA

## 175. Antes de activar

- [ ] Código correcto.
- [ ] Símbolo correcto.
- [ ] Decimales correctos.
- [ ] Conversión disponible.
- [ ] Fuente identificada.
- [ ] Presupuesto probado.
- [ ] Pagos probados cuando corresponda.
- [ ] Reembolsos probados cuando corresponda.

---

# CD. CHECKLIST DE NUEVO MERCADO

## 176. Producto

- [ ] Calidad suficiente.
- [ ] Idioma.
- [ ] Moneda.
- [ ] Destinos.
- [ ] Engine probado.

---

## 177. Comercial

- [ ] Pagos.
- [ ] Afiliados.
- [ ] Pricing.
- [ ] Potencial económico.

---

## 178. Legal

- [ ] Privacidad.
- [ ] Términos.
- [ ] Consumidor.
- [ ] Cookies.
- [ ] Impuestos revisados.

---

## 179. Operación

- [ ] Soporte.
- [ ] Proveedores.
- [ ] Monitoreo.
- [ ] Costos.
- [ ] Incidentes.

---

# CE. SEÑALES PARA EXPANDIR

## 180. Positivas

- Usuarios llegan desde otro mercado.
- Solicitan idioma.
- Crean viajes.
- Buena calidad del Engine.
- Existe potencial comercial.
- Datos suficientes.

---

# CF. SEÑALES PARA ESPERAR

## 181. Negativas

- Baja calidad de datos.
- Problemas de idioma.
- Demasiado soporte.
- Costos altos.
- Riesgos regulatorios.
- Poca demanda.
- Mala conversión.

---

# CG. PRIORIDAD DE EXPERIENCIA

## 182. Principio

Un usuario internacional no debería sentir que está utilizando una versión secundaria del producto.

---

## 183. Estándar

Cuando ZAREVOA anuncie oficialmente soporte para un idioma o mercado, deberá intentar ofrecer una experiencia suficientemente completa.

---

# CH. VENTAJA ESTRATÉGICA

## 184. Potencial

La internacionalización puede convertirse en una ventaja si ZAREVOA logra combinar:

- Travel Profile.
- Engine.
- Datos internacionales.
- Localización.
- Monedas.
- Proveedores.
- Aprendizaje.

---

## 185. Objetivo

Que el mismo sistema pueda comprender a viajeros de distintos países sin producir una experiencia genérica.

---

# CI. VISIÓN DE LARGO PLAZO

## 186. Experiencia

Un viajero debería poder abrir ZAREVOA desde su país, utilizar su idioma y moneda, viajar a otra región del mundo y seguir comprendiendo toda la planificación.

---

## 187. Ejemplo conceptual

**Usuario en Chile**

↓

**ZAREVOA en español**

↓

**Presupuesto en CLP**

↓

**Viaje por Japón**

↓

**Costos locales en JPY con referencia comprensible**

↓

**Horarios en hora local**

↓

**Journey durante el viaje**

Todo deberá funcionar como una sola experiencia.

---

# CJ. PRINCIPIO FINAL

## 188. Internacionalización con criterio

ZAREVOA no deberá intentar conquistar todos los mercados simultáneamente.

Deberá construir primero una arquitectura que permita crecer y después expandirse donde exista una combinación adecuada de:

**demanda + calidad + datos + capacidad + sostenibilidad.**

---

## 189. Regla final

La estrategia internacional deberá seguir este orden:

**Preparar**

↓

**Localizar**

↓

**Probar**

↓

**Validar**

↓

**Lanzar**

↓

**Medir**

↓

**Mejorar**

↓

**Expandir**

La meta no será poder decir:

**“ZAREVOA está disponible en todo el mundo.”**

La meta será que, cuando ZAREVOA entre oficialmente en un mercado, el viajero sienta:

**“ZAREVOA funciona para mí, aunque mi viaje cruce el mundo.”**

---

**Estado del documento:** Plan oficial inicial de internacionalización, idiomas, monedas y expansión de mercados de ZAREVOA.
