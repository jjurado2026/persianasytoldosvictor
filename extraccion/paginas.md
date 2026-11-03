# Mapa del sitio — persianasytoldosvictor.es

Extraído el 03/11/2026 de `robots.txt` → `wp-sitemap.xml` (índice con 4 sub-sitemaps: posts, pages, metform-form, category) + navegación principal + pie. Plataforma: WordPress, tema Hello Elementor 2.8.1, Elementor 3.16.5, cabecera y pie hechos con Jeg Elementor Kit (plantillas Elementor 58 y 194).

13 URLs públicas en total: 7 son páginas reales del negocio, y las otras 6 son restos de la instalación que se indexan (ver «Residuales»).

## Navegación

- **Menú principal** (cabecera, en todas las páginas): Inicio `/` · Sobre nosotros `/sobre-nosotros` · Contacto `/contacto` · Términos y condiciones `/terminos-y-condiciones`
- **Pie** (en todas las páginas): Política de cookies `/politica-de-cookies` · Aviso Legal `/aviso-legal` · Política de Privacidad `/politica-de-privacidad` (las tres con `target="_blank"`)
- **Botones internos:** «Contactar» → `/contacto` (home y sobre-nosotros)
- No hay enlaces a redes sociales, WhatsApp ni teléfono clicable en ninguna página.

## Páginas del negocio

| # | URL | `<title>` | Plantilla | Última modificación (sitemap) |
|---|---|---|---|---|
| 1 | `/` | persianasytoldosvictor – Just another WordPress site | Elementor full width (página 26) | 09/05/2023 |
| 2 | `/sobre-nosotros` | Sobre nosotros – persianasytoldosvictor | Elementor full width (61) | 13/04/2023 |
| 3 | `/contacto` | Contacto – persianasytoldosvictor | Elementor full width (63) | 20/04/2023 |
| 4 | `/terminos-y-condiciones` | Términos y condiciones – persianasytoldosvictor | Página WP por defecto (Complianz T&C) | 12/02/2024 |
| 5 | `/politica-de-privacidad` | Política de privacidad – persianasytoldosvictor | Página por defecto + Elementor (291) | 20/04/2023 |
| 6 | `/politica-de-cookies` | Política de cookies – persianasytoldosvictor | Página por defecto + Elementor (299) | 20/04/2023 |
| 7 | `/aviso-legal` | Aviso legal – persianasytoldosvictor | Página por defecto + Elementor (304) | 20/04/2023 |

## Residuales (indexados en el sitemap, sin enlazar desde la web)

| URL | `<title>` | Qué es |
|---|---|---|
| `/sample-page` | Sample Page – persianasytoldosvictor | Página de ejemplo de WordPress, en inglés, con enlace a `/wp-admin/` |
| `/archivos/1` | Hello world! – persianasytoldosvictor | Entrada de ejemplo «Hello world!» con el comentario de ejemplo y el formulario de comentarios abierto |
| `/archivos/category/uncategorized` | Uncategorized – persianasytoldosvictor | Archivo de la categoría por defecto |
| `/archivos/metform-form/new-form-1678890069` | Formulario presupuesto – persianasytoldosvictor | El formulario de la home, publicado como página suelta |
| `/archivos/metform-form/new-form-1679413956` | New Form # 1679413956 – persianasytoldosvictor | Formulario de plantilla sin usar, en inglés («Simple Contact Form», First Name, Last Name…) |
| `/archivos/metform-form/new-form-1679486027` | Formulario página de contacto – persianasytoldosvictor | El formulario de /contacto, publicado como página suelta |
| (cualquier URL inexistente) | Página no encontrada – persianasytoldosvictor | 404 genérica del tema: «No se ha podido encontrar la página.» |

---

## Elementos globales (en todas las páginas)

### Cabecera (plantilla Elementor 58, `header#masthead`, no es sticky)
Sección encajada a 1140 px, 2 columnas al 50 %, sin fondo (se ve blanco).
- **Col. 1:** H2 de texto «Persianas y Toldos Víctor», que hace de logotipo. Verde oliva `#767522`, fuente del sistema a 32 px y peso 500. **No enlaza a la home** y no hay logotipo en imagen.
- **Col. 2:** menú de Jeg Kit (`jkit_nav_menu`) con 4 enlaces en Verdana 700 a 14 px. Color burdeos `#820933`; el activo y el hover, en oliva `#767522`. Por debajo de 1024 px pasa a botón hamburguesa (`aria-label="open-menu"`) que abre un panel lateral izquierdo de 360 px con fondo `#F7F7F7`, un enlace de logo vacío (sin texto ni imagen) y un botón de cierre (`aria-label="close-menu"`).

### Pie (plantilla Elementor 194, `<footer>`)
Fondo verde oliva `#767522` (color global primario) y 3 columnas al 33 %, con todo el texto en blanco y Nunito.
- **Col. 1:** H3 «quienes somos», en mayúsculas por CSS, con tracking de 4 px y corchetes `[ ]` ámbar `#FFAB00` añadidos con `::before`/`::after`. Debajo, el texto «Instalación y reparación de persianas y toldos en Valencia».
- **Col. 2:** H3 «horario» y 7 párrafos con el horario de lunes a domingo (copiado de Google: los `<span class="WF8WNe">` son clases de la ficha de Google).
- **Col. 3:** H3 «Contacto» y una lista de iconos con 2 ítems (dirección y teléfono), cuyos iconos están vacíos. Debajo, otra lista con los 3 enlaces legales.
- Sin copyright, logo, redes, mapa ni CTA.

### Banner de cookies (Complianz GDPR)
Al entrar aparece un modal centrado de 550×260 px con el título «Gestionar el consentimiento de las cookies», un texto, los botones «Aceptar» (azul `#1E73BE`, el azul por defecto de WP, fuera de la marca) y «Ver preferencias», y 3 enlaces legales. **El botón «Denegar» existe en el HTML pero no se ve en la primera capa.** Tras aceptar queda una pestaña fija «Gestionar consentimiento» abajo a la derecha, que tapa campos del formulario a 390 px y la tarjeta del hero de Sobre nosotros a 1440 px. El mapa de Google de /contacto está bloqueado hasta aceptar (categoría marketing).

---

## 1. HOME `/` — bloques en orden (para remaquetar 1:1)

Medidas a 1440 px: documento de 4.830 px de alto; a 390 px, 9.339 px. Contenedor encajado de 1140 px. Las animaciones son las de entrada de Elementor (`fadeIn` con retardos de 50 a 400 ms y un `pulse`), sin coreografía propia.

### Bloque 0 · Cabecera
Ver «Elementos globales».

### Bloque 1 · Hero con formulario de presupuesto (`60f85353`)
- **Tipo:** hero a pantalla completa (`height-full`, es decir, al menos 100vh), ancho completo, contenido centrado en vertical, 2 columnas al 50 %. Padding de 260 px arriba y 240 px abajo.
- **Fondo:** imagen CSS `omar-sotillo-franco-HkO7lnpJcvA-unsplash-scaled.jpg`, de stock (fachada de madera amarilla con un toldo de rayas rojas y blancas), con `background-position: 0 -356px` en escritorio y `0 0` en tablet y móvil. Overlay negro al 50 %. Es el elemento LCP.
- **Col. 1:**
  - H2 «PERSIANAS Y TOLDOS VÍCTOR»: Quicksand 700, 50/61 px, verde lima `#D4E79E`; 33 px en móvil.
  - H2 «VENTA, INSTALACIÓN Y REPARACIÓN DE TOLDOS Y PERSIANAS EN VALENCIA»: Mulish 500, 24/35 px, blanco; 18 px en móvil.
- **Col. 2:** formulario MetForm n.º 28 («Formulario presupuesto»), que se monta con JS (React + `htm`).
  - Tarjeta blanca con radio de 20 px y H2 «PEDIR PRESUPUESTO» en oliva `#767522` (fuente del sistema, 32 px).
  - Campos: Nombre y Teléfono en una fila; «Email» y «Email» en otra (el segundo es el campo `mf-subject` con el placeholder equivocado); textarea «¿Cómo podemos ayudarte?».
  - Casilla RGPD (que no es obligatoria) y botón «Obtener presupuesto» (fondo burdeos `#820933`, texto blanco, Roboto 500 a 14 px).
  - Los campos, en IBM Plex Sans, con fondo `#F6F7FA` y radio de 6 px.
- **A 1440×900:** el titular queda a media altura, a la izquierda; el formulario, a la derecha, entre y=315 y 765. En móvil se apilan: la foto se recorta y solo se ve la pared amarilla.

### Bloque 2 · Experiencia + 3 ventajas (`35f3fc90`)
- **Tipo:** 2 columnas encajadas, con padding de 40 px y fondo blanco.
- **Col. 1:**
  - H2 «Más de 60 años de experiencia»: Quicksand 700, 35/61 px, negro.
  - Garabato decorativo `graphic-2.png` (212×202, en posición absoluta, oculto en móvil), restos de la plantilla.
  - Imagen `sara-sadeghloo-A8bjSrQg9CQ-unsplash-scaled.jpg` (2560×1920, con srcset y `fetchpriority=high`), de stock: terraza de un hotel bajo una pérgola con lona beige y un olivo. Sin alt.
- **Col. 2:** 3 sub-secciones apiladas, cada una con una tarjeta blanca con sombra (icon box de Jeg Kit con solo el H3, sin descripción) y, a su izquierda, un icono cuadrado burdeos `#820933` con glifo blanco de 32 px:
  1. H3 «Servicio rápido», con el icono `jki-flash-light` (rayo).
  2. H3 «Profesionales», con el icono `jki-Mechanic-light` (operario).
  3. H3 «Ahorro y Calidad», con el icono `jki-phone-call-line`: un teléfono, que no corresponde al texto.
- Títulos en Mulish 700 a 23 px, en oliva.
- En móvil, el icono se separa de su tarjeta y queda desalineado.

### Bloque 3 · Ofertas (`31deb4e1`)
- **Tipo:** banda a ancho completo con fondo `linear-gradient(270deg, #820933 27%, #D4E79E3B 18%)`. La columna interior es burdeos `#820933` y se ve toda la banda burdeos. El `margin-top` está mal escrito (`0100px`).
- **Sub-sección 1** (2 columnas):
  - La columna izquierda está vacía.
  - En la derecha va el párrafo «Estate atento a todas nuestras ofertas y novedades en la web!» (Quicksand 600, 30 px, lima `#D4E79E`) y una flecha decorativa `graphic-arrow-2.png`, en posición absoluta, girada 103° y oculta en tablet y móvil.
- **Sub-sección 2** (con `fadeIn`): 2 tarjetas *image box* (imagen a la izquierda, texto a la derecha, fondo blanco):
  1. **Imagen:** miniatura recortada de `persianas-toldos-victor-12.jpg`, foto real de un toldo blanco en un balcón, con alt «persianas-toldos-victor-12».
     **Título:** «20% de descuento en toldos» (Quicksand 800, 18 px, `#0C0C0C`).
     **Texto:** «Toldos stor para balcon con un 20% de descuento de 15/02/23 al 15/03/23» (14 px, gris `rgba(122,122,122,.69)`, fuente «Muli», que no se carga). **Oferta caducada desde marzo de 2023.**
  2. **Imagen:** miniatura de `2022-12-14.jpg`, foto real de una mampara de ducha, con alt «2022-12-14».
     **Título:** «Mampara ducha desde 190€».
     **Texto:** «MAMPARA FIJA DUCHA CRISTAL TEMPLADO EN 48H DESDE 190€».
- En móvil, el texto promocional toca el borde izquierdo de la pantalla, sin margen.

### Bloque 4 · Nuestros servicios (`404a24c2`)
- **Tipo:** sección a ancho completo, blanca, con padding de 80 px arriba y 10 px abajo. Dentro, una sub-sección encajada de 2 columnas.
- **Col. 1:** imagen `persianas.png` (460×310, PNG de 272 KB), una mano abriendo una puerta con veneciana. Tiene aspecto de stock. Sin alt.
- **Col. 2:** H3 «NUESTROS SERVICIOS» (Quicksand 700, 35 px, negro) y una lista con iconos `fa-check` burdeos, con 7 ítems. El texto va en oliva, en la fuente del sistema a 16 px, y en burdeos al pasar el ratón.
  1. Venta, reparación e instalación de persianas y toldos
  2. Mosquiteras
  3. Rejas
  4. Stores
  5. Ventanas
  6. Mamparas de ducha y bañera
  7. Motorización de persianas y toldos
- Los ítems no enlazan a nada: no hay páginas de servicio.

### Bloque 5 · CTA «Te asesoramos sin compromiso» (`7dd0b3a2`)
- **Tipo:** banda de CTA centrada, con padding de 100 px.
- **Fondo:** imagen `rooted-studio-O6T_Fc11M9Q-unsplash-scaled.jpg`, de stock (toldo azul de un comercio contra el cielo), con `background-attachment: fixed` (parallax) y overlay `#0C0200` al 75 %. Se ve casi marrón oscuro.
- H2 «Te asesoramos sin compromiso»: Roboto 500, 60 px (48 en tablet, 40 en móvil), blanco, con `fadeIn` de 100 ms.
- H2 «VENTA, INSTALACIÓN Y REPARACIÓN DE TOLDOS Y PERSIANAS EN VALENCIA»: Roboto 400, 20 px, blanco, con `fadeIn` de 200 ms. **Es el mismo texto que el subtítulo del hero.**
- Botón «Contactar» → `/contacto`:
  - lima `#D4E79E` con texto negro, borde oliva de 1 px y forma de píldora (radio 24 px);
  - en hover, fondo blanco y texto oliva;
  - `fadeIn` de 400 ms.

### Bloque 6 · Testimonios (`2c7a4576`)
- **Tipo:** sección estirada, con fondo blanco y overlay blanco al 93 %. La columna lleva padding de 30, 50, 80 y 80 px.
- H2 «Que opina la gente de nosotros» (Quicksand 700, 35 px), seguido de un espaciador.
- **3 tarjetas** en columnas al 33 %, con fondo lima `#D4E79E`, padding de 2em y texto centrado en cursiva (Nunito Sans, 17,6/29,9 px, negro). El nombre va en burdeos, con tracking de 1 px.
  1. «Sin duda ha sido un acierto contar con ellos…», de Arantxa V
  2. «Muy buenos profesionales…», de María P
  3. «Excelente atención, el chico es un gran profesional…», de SONIA D
- **Las 3 tarjetas tienen alturas distintas.** No llevan foto, estrellas, fecha ni fuente (no consta si son de Google).
- Debajo, 2 espaciadores.

### Bloque 7 · Cabecera del porfolio (`e235cfb`)
- H2 «Nuestro trabajo», como antetítulo: Mulish 400, 20 px, burdeos, con `fadeIn`.
- H2 «Porfolio»: Quicksand 700, 35 px, negro.

### Bloque 8 · Galería del porfolio (`50d2b873` + `5a97eb98`)
- **Tipo:** mosaico de 7 fotos reales del cliente, repartido en 2 secciones encajadas de 2 columnas cada una:
  - **Fila A.** Col. izquierda al 50 %: `porfolio-01` grande y cuadrada. Col. derecha al 50 %: `porfolio-02` horizontal y, debajo, 2 columnas con `porfolio-03` y `porfolio-04`.
  - **Fila B.** Col. izquierda al 50 %: 2 columnas con `porfolio-05` y `porfolio-06`. Col. derecha al 50 %: `porfolio-07`, horizontal.
- Son miniaturas recortadas de Elementor sobre originales de 960×960.
- Cada imagen está dentro de `<a href="#">`, un enlace muerto, sin lightbox ni pie de foto. Los alt son los nombres de archivo («persianas-toldos-victor-4», «persianas-toldos-victor-&», etc.).
- Entran con `fadeIn` escalonado de 100 a 400 ms.
- `porfolio-05` es la misma foto que la tarjeta de oferta 1.

### Bloque 9 · Pie
Ver «Elementos globales».

---

## 2. SOBRE NOSOTROS `/sobre-nosotros`

1. **Hero partido (`780b334`):** ancho completo, fondo oliva `#767522`, 2 columnas.
   - **Col. 1:** columna con imagen de fondo `roller-blinds-on-balcony-windows-…-utc-scaled.jpg` (stock de Envato: estores noche y día en una habitación blanca) y un espaciador.
   - **Col. 2:** dos sub-secciones:
     - Una con el H1 «Expertos en toldos y persianas desde 1963» (lima `#D4E79E`, fuente del sistema, 40 px) y el párrafo blanco «Nos basamos en un trato familiar…».
     - Otra de 2 columnas: a la izquierda, sobre lima, el H3 «Más de 60 años de experiencia» y el texto «Trabajamos con todo tipo de proveedores y fabricantes.»; a la derecha, la imagen de fondo `victoire-joncheray-…-unsplash-scaled.jpg` (stock: fachada con toldos naranjas vista desde abajo).
2. **«Te hacemos la vida más fácil» (`703d1e45`):** 2 columnas.
   - **Izquierda:** imagen `sara-sadeghloo` (la misma de la home) y el garabato decorativo.
   - **Derecha:** H2 en Verdana 800, 32 px, oliva; un párrafo; y una lista con 3 iconos (check, saco de dinero, flecha arriba): Garantía, Buen precio garantizado y Materiales de alta calidad.
3. **CTA «Consúltenos…» (`2a41c31e`):** 2 columnas.
   - **Izquierda:** imagen de fondo `adam-birkett-…-unsplash-scaled.jpg` (stock: toldo de rayas contra el cielo).
   - **Derecha**, sobre lima:
     - H2 en Verdana 700, oliva;
     - flecha decorativa;
     - párrafo;
     - botón «Contactar» → `/contacto`, burdeos y cuadrado, con padding de 22 × 40 px, que se vuelve oliva en hover y se desplaza 10 px a la derecha.
4. **Pie.**

## 3. CONTACTO `/contacto`

1. **Cabecera (`7869848e`):** fondo lima `#D4E79E`, texto centrado y animaciones `fadeIn`.
   - H2 «Estamos encantados de ayudarte», como antetítulo: Roboto 500, 12-16 px, en mayúsculas, oliva.
   - H2 «Contacta con nosotros»: Roboto 500, 3rem, burdeos.
   - Divisor oliva de 4 px.
   - H2 «Nos pondremos en contacto con usted lo antes posible»: Roboto 18 px, `rgba(0,0,0,.54)`.
2. **Mapa, datos y formulario (`2661a5f3`):** 2 columnas.
   - **Col. 1:**
     - Google Maps (iframe con «Calle Lladró y Malli, 12 46007 Valencia», zoom 10: se ve media provincia en lugar de la calle; bloqueado por Complianz hasta aceptar las cookies).
     - Debajo, 2 columnas:
       - **«datos de contacto»:** H2, con iconos de marcador, teléfono y sobre. Dirección, «963413713» sin `tel:` y el email con `mailto:`.
       - **«HORARIO»:** H2 y 7 líneas.
   - **Col. 2** (con animación `pulse`): formulario MetForm n.º 139 («Formulario página de contacto»), que se monta con JS.
     - H3 «¿Cómo podemos ayudarte?» y un párrafo.
     - Campos con label: Nombre\*, Teléfono\*, Email\* y Consulta\*.
     - Casilla RGPD y botón «Enviar» (lima con texto burdeos).
     - Usa IBM Plex Sans, fuera del resto de la web.
3. **Pie.**

## 4. TÉRMINOS Y CONDICIONES `/terminos-y-condiciones`
Página por defecto del tema, generada por el plugin Complianz Terms & Conditions. H1 y 22 apartados en H2 («1. Introducción» … «22. Descargar»), con un enlace al formulario de desistimiento en PDF y otro para descargar los términos en PDF. Sin Elementor.

## 5-7. POLÍTICA DE PRIVACIDAD, POLÍTICA DE COOKIES, AVISO LEGAL
Las tres siguen la misma plantilla: sección con el título en H2 (sin H1), una sección de texto (widget de editor de texto) con apartados en H3 y el pie.
