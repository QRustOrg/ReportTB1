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