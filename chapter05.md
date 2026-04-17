# Capitulo V: Solution UX/UI Design

## 5.1 Product Design

### 5.1.1 Style Guidelines

En esta sección, el equipo establece la estética y marca de identidad visual del producto (assets, fonts,
colores, iconografía) para mantener una presentación alineada con el espíritu de Klippr: dinámico, confiable y cercano a nuestros clientes.

#### 5.1.1.1 General Style Guidelines

**Branding**

* Identidad visual cercana que transmite **confianza**, **seguridad anti-fraude** y **comunidad**: La estética combina energía juvenil (paleta vibrante, mascota slime) con señales de credibilidad (validación QR, reseñas verificadas), apelando a usuarios de 18–45 años en América Latina.
* Cada elemento visual refuerza el core de la app usando iconografía intuitiva: QR's, etiquetas de descuento, estrellas de rating y burbujas de comunidad; claros, simples y reconocibles en pantallas móviles de cualquier tamaño.

**Typography**

* Tipografías Montserrat para alta legibilidad optimizada para dispositivos móviles.
* Sistema de jerarquía:
    * **Titulos Principales**: Bold, tamaño grande para encabezados.
    * **Subtitulos**: Semi-bold, para secciones y tarjetas.
    * **Texto General**: Regular, tamaño legible para contenido de lectura.
    * **Labels**: Medium, tamaño mediano para etiquetas.
    
**Colors**

* Paleta de colores basada en tonos violeta/púrpura como principales.
    * **Primario**: Violeta(#7161ef) - botones principales, elementos activos.
    * **Secundarios**: Tonos claros (#957fef) de lila para fondos.
    * **Neutros**: Blancos, negros y grises claros para tarjetas y textos.
    * **Acentos**: Verde para estados de éxito y rojo para alertas.

**Spacing**

* Sistema de espaciado para mantener ritmo visual consistente en cada pantalla:
    * **Micro (4px)**: separación entre ícono y etiqueta, gaps internos de chips y badges de descuento.
    * **Small (8px)**: padding interno de botones secundarios y separación entre líneas de metadata (vigencia, categoría).
    * **Base (16px)**: margen horizontal estándar de pantalla; padding interno de tarjetas de promoción y QR.
    * **Medium (24px)**: separación entre secciones del feed, entre tarjeta y barra de navegación inferior.
    * **Large (32–48px)**: espaciado de pantallas vacías (estados de cero resultados) y separación de bloques en dashboards de empresa.

**Communication Tone**

* **Cercano y directo**: Klippr habla como un amigo que te avisa de una buena oferta, nunca como una entidad corporativa. Se usa segunda persona informal (*"Tu QR está listo"*, *"¡Canje exitoso!"*).
* **Breve y accionable**: los microtextos (botones, toasts, notificaciones push) priorizan la acción sobre la descripción. Máximo 2 líneas en cualquier mensaje de interfaz.
* **Confiable sin ser rígido**: los mensajes de validación comunican seguridad con lenguaje positivo (*"Código verificado ✓"*) evitando términos técnicos que generen fricción.
* **Inclusivo**: redacción neutral en género donde sea posible.

**Dimension Guidelines**

* Todos los componentes siguen una grilla de **4 columnas** en móvil (360–414px de ancho) con márgenes de 16px y 8px.
* **Tarjetas de promoción**: ancho 100% del contenedor, altura mínima de 120px.
* **Botón primario (CTA)**: altura fija de **48px**, ancho mínimo de 160px.
* **Ícono QR y scanner overlay**: área de escaneo centrada de **240×240px** con esquinas guía de 24px; margen de seguridad de 32px respecto a bordes de pantalla.
* **Avatar / logo de empresa**: tamaño estándar de **40px** en feed y **72px** en perfil de negocio; forma circular con borde de 2px en color primario.
* **Bottom navigation bar**: altura de **64px** con íconos de 24px y labels de 10px, siempre visible durante el flujo de descubrimiento y canje.

### 5.1.2 Information Architecture

#### 5.1.2.1 Organization Systems

La arquitectura de información de Klippr organiza el contenido tanto en la landing page como en la aplicación móvil.

**Jerárquico (Visual Hierarchy)**

La landing page aplica jerarquía visual descendente desde la propuesta de valor general hacia los detalles específicos por segmento. 

En la aplicación móvil, la jerarquía visual organiza cada pantalla en tres zonas: encabezado de navegación, área de contenido principal y barra de navegación inferior fija.

**Secuencial (Step-by-Step)**: Implementado en:

* Proceso de registro de usuario
* Descubrir una promoción
* Generar el código QR
* Canjearlo en el punto de venta 
* Dejar una reseña.

**Por Topicos**

El contenido de la landing se organiza por tópicos temáticos agrupados por afinidad:

* Problema (Sección 2)
* Solución funcional (Sección 3) 
* Valor por segmento (Sección 4) 
* Evidencia social y métricas (Sección 5)
* Posicionamiento competitivo (Sección 6). 

**Segun Audiencia**

* **Usuarios**: acceso al feed de promociones, generación de QR, historial de canjes y módulo social (reseñas, calificaciones, notificaciones).
* **Empresas**: acceso al dashboard de campañas, panel de validación de QR en punto de venta y sección de respuesta a reseñas.

#### 5.1.2.2 Labelling Systems

El sistema de etiquetas de Klippr prioriza claridad y brevedad sobre descripción exhaustiva. Las etiquetas emplean el vocabulario cotidiano del contexto latinoamericano (canjear, promo, descuento, oferta) en lugar de términos técnicos. 

**Ejemplos de Etiquetas**

| Elemento | Etiqueta | Tipo |
|---|---|---|
| Pestaña principal de contenido | Descuentos | Navegacion |
| Pestaña de busqueda | Buscar | Navegacion |
| Pestaña de actividad personal | Mis canjes | Navegacion |
| Pestaña de cuenta | Perfil | Navegacion |
| Boton de activacion de descuento | Obtener descuento | Accion |
| Boton de confirmacion de canje | Canjear ahora | Accion |
| Boton de envio de resena | Publicar resena | Accion |
| Estado del codigo QR activo | Pendiente | Estado |
| Estado del codigo QR utilizado | Canjeado | Estado |
| Estado del codigo QR vencido | Expirado | Estado |
| Filtro de categoria en el feed | Categoria | Filtro |
| Filtro de proximidad geografica | Cerca de ti | Filtro |
| Filtro de porcentaje minimo | Descuento minimo | Filtro |
| Indicador de calificacion | Rating | Label |
| Seccion de opiniones de usuarios | Resenas | Label |
| Panel de metricas del negocio | Resultados | Label |
| Metrica de vistas de campana | Vistas | Label |
| Metrica de canjes realizados | Canjes | Label |

**Asociaciones**

Las etiquetas mantienen correspondencia con los estados y acciones del sistema para evitar ambiguedad. El estado "Pendiente" siempre indica un QR generado pero no validado. El estado "Canjeado" siempre indica un QR bloqueado tras validacion exitosa. La accion "Obtener descuento" siempre precede a la generacion del QR. La accion "Canjear ahora" siempre ocurre en el punto de venta con el QR activo en pantalla.

En el dashboard del negocio, las etiquetas de metricas guardan relacion directa con el evento que representan: "Vistas" corresponde a los accesos al detalle de la campana; "Canjes" corresponde a los QR validados exitosamente; "Rating" corresponde al promedio ponderado de calificaciones de resenas vinculadas a canje completado.

#### 5.1.2.3 SEO Tags and Meta Tags

**Landing Page**

* **Title:** "Klippr — Descuentos con QR unico, anti-fraude y comunidad"
* **Meta description:** "Conecta usuarios y negocios mediante descuentos seguros con codigo QR único."
* **Keywords:** "descuentos, cupones digitales, QR unico, anti-fraude, ofertas verificadas, resenas de descuentos, app de promociones, PYMEs, canjes seguros, descuentos LATAM, Klippr, QRust"
* **Author:** QRust

**Aplicacion Movil**

* **Title:** "Klippr — Descuentos seguros con QR"
* **Meta description:** "Descubre ofertas reales cerca de ti, genera tu QR unico y canjea en tienda en menos de 3 segundos. Resenas verificadas de tu comunidad para decidir con confianza."

#### 5.1.2.4 Searching Systems

Klippr implementa un sistema de busqueda multicapa que permite al usuario consumidor encontrar promociones relevantes por distintos criterios sin necesidad de navegar por el feed completo.

El primer nivel de busqueda es la **busqueda por texto libre**, que opera sobre el nombre del negocio, la categoria y el titulo de la promocion. La busqueda se ejecuta con debounce de 300ms para evitar peticiones innecesarias y devuelve resultados ordenados por relevancia combinada (coincidencia en nombre de negocio tiene mayor peso que coincidencia en descripcion de campana).

El segundo nivel es el **filtrado por facetas**, que permite al usuario refinar resultados por categoria de negocio (restaurantes, retail, servicios, entretenimiento), por rango de porcentaje de descuento, por proximidad geografica (requiere permiso de ubicacion; si no se otorga, el filtro por proximidad se desactiva sin bloquear el resto de la experiencia) y por estado de vigencia (activa, por vencer en menos de 24 horas).

El tercer nivel es el **ordenamiento**, que permite al usuario reordenar los resultados por mayor porcentaje de descuento, por rating promedio de resenas o por distancia al punto de venta (si la ubicacion esta disponible).

En el contexto del negocio afiliado, el sistema de busqueda dentro del dashboard permite filtrar campanas propias por estado (activa, pausada, finalizada) y por rango de fechas de publicacion. La busqueda en el panel de validacion de QR soporta ingreso manual del codigo alfanumerico como alternativa al escaneo por camara, cubriendo la variabilidad de condiciones de los puntos de venta.

#### 5.1.2.5 Navigation Systems

**Landing Page**

La landing aplica navegacion de una sola pagina (single-page) con scroll vertical continuo. La barra de navegacion superior es fija (sticky) y visible en todo momento. Contiene el logotipo de Klippr (ancla al inicio de la pagina) y, en su extremo derecho, dos elementos de navegacion: un enlace de texto "Para negocios" que ejecuta scroll suave hacia la seccion de beneficios con el tab B2B preseleccionado, y el boton primario "Descarga la app" que dirige al store correspondiente segun el sistema operativo del dispositivo detectado. En resolucion movil, el boton "Para negocios" colapsa dentro de un menu hamburguesa.

Los dots de progreso de scroll (indicadores de seccion) son opcionales y se evaluan segun el feedback de usabilidad del MVP. Si se implementan, aparecen como una barra lateral derecha discreta en desktop.

**Aplicacion Movil (Consumidor)**

La navegacion principal utiliza una barra inferior fija de cinco elementos: feed de descuentos, busqueda, generador de QR (elemento central con mayor jerarquia visual, representado por un boton flotante con radio de 28px sobre la barra), historial de canjes y perfil de usuario. Esta estructura de navegacion plana permite acceder a cualquier modulo principal en un solo tap desde cualquier pantalla del flujo.

La navegacion secundaria opera mediante hojas deslizables desde la parte inferior (bottom sheets) para filtros, detalles de promocion y acciones contextuales, preservando el contexto del feed sin romper el flujo de navegacion. Las acciones destructivas o de alta consecuencia (como cancelar un QR activo) se confirman mediante un dialogo modal antes de ejecutarse.

**Aplicacion Movil (Negocio)**

El negocio afiliado accede a una navegacion diferenciada que reemplaza el feed de descuentos por el dashboard de campanas y el historial de canjes por el panel de validacion de QR. La estructura de barra inferior mantiene el mismo patron de cinco elementos para coherencia de la plataforma, pero con iconografia y etiquetas especificas al rol del negocio. La pantalla de validacion de QR (escaneo o ingreso manual) se accede desde el elemento central de la barra, con el mismo patron de jerarquia visual que el generador de QR del consumidor, subrayando la simetria funcional entre ambos roles en el momento del canje.