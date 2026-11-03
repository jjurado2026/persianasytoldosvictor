# Identidad extraída — Persianas y Toldos Víctor

Fuentes de la extracción:
- CSS del kit de Elementor (`wp-content/uploads/elementor/css/post-5.css`) y de cada página (post-26, 58, 61, 63, 194, 28 y 139).
- Estilos calculados con `playwright-cli -s=persianasytoldosvictor eval` + `getComputedStyle` a 1440×900, tras aceptar las cookies.

## Logotipo

- **No existe logotipo en imagen ni en SVG.** El «logo» es un H2 de texto, «Persianas y Toldos Víctor», en oliva `#767522` y con la fuente del sistema (`-apple-system, system-ui, Segoe UI, Roboto…`) a 32 px y peso 500. Se ve distinto en Mac, en Windows y en Android, y no enlaza a la home.
- La biblioteca de medios (78 archivos, consultada por la API REST) no contiene ningún archivo de logo.
- El panel del menú móvil tiene un enlace de logo vacío (`a.jkit-nav-logo`), sin imagen ni texto.
- **Pendiente:** pedir al cliente el logo en vector, si lo tiene (rótulo del local, furgoneta, facturas). Si no lo tiene, el rediseño trabajará con un logotipo tipográfico a partir del nombre, presentado como propuesta aparte y sin aplicarse sin OK.

## Favicon, iconos y OG

| Recurso | Estado | Archivo guardado |
|---|---|---|
| Favicon | No hay `<link rel="icon">`. `/favicon.ico` redirige (302) al logo gris por defecto de WordPress, `wp-includes/images/w-logo-gray-white-bg.png` (80×80) | `assets/originales/favicon-wordpress-por-defecto.png` (no es de la marca) |
| apple-touch-icon | No existe (404) | — |
| og:image / og:* / twitter:* | No hay ninguna etiqueta Open Graph ni Twitter en ninguna página | — |
| `theme-color` | `#FFFFFF` | — |

## Colores

### Variables globales de Elementor (`.elementor-kit-5`)

| Variable | Hex | Nombre | Uso real |
|---|---|---|---|
| `--e-global-color-primary` (y su duplicado `--e-global-color-148c611`) | **`#767522`** | Verde oliva | Logo de texto, enlace activo del menú, fondo del pie y del hero de Sobre nosotros, texto de la lista de servicios, títulos de las ventajas, divisor de Contacto, cabecera del formulario |
| `--e-global-color-secondary` (y `--e-global-color-dbda567`) | **`#D4E79E`** | Verde lima pálido | Titular del hero, tarjetas de testimonios, botón «Contactar» de la home, fondo de la cabecera de Contacto y de bloques de Sobre nosotros, botón «Enviar» |
| `--e-global-color-accent` (y `--e-global-color-0b6eb30`) | **`#820933`** | Burdeos | Enlaces del menú, banda de ofertas, iconos cuadrados, checks de servicios, botón «Obtener presupuesto», nombres de los testimonios, H2 «Contacta con nosotros» |
| `--e-global-color-text` | `#000000` | Negro | Títulos de sección y texto de los testimonios |

Las tres variables duplicadas tienen el mismo valor: alguien creó los colores «personalizados» repitiendo los globales.

### Otros colores en uso (calculados o del CSS)

| Hex | Uso |
|---|---|
| `#FFFFFF` | Fondo general (`body`), texto sobre oliva y sobre las fotos |
| `#333333` | Texto de cuerpo por defecto del tema Hello Elementor |
| `#0C0C0C` | Títulos de las tarjetas de oferta |
| `rgba(122,122,122,.69)` ≈ `#A3A3A3` | Descripción de las tarjetas de oferta |
| `rgba(0,0,0,.54)` ≈ `#757575` | Subtítulo de Contacto |
| `#CC3366` | Color de enlace por defecto del tema (enlace «Política de Privacidad» del formulario). No es de la marca |
| `#FFAB00` | Corchetes `[ ]` de los títulos del pie y hover de los enlaces del pie |
| `#F6F7FA` / `#0D1427` / `#878991` | Fondo, texto y placeholder de los campos de MetForm |
| `#54565C` | Párrafo del formulario de Contacto |
| `#F7F7F7` | Panel del menú móvil |
| `#000000` al 50 % | Overlay del hero |
| `#0C0200` al 75 % | Overlay del CTA «Te asesoramos» |
| `#1E73BE` | Botón «Aceptar» del banner de cookies (azul por defecto de WP, fuera de la marca) |
| `#FF0000` | Asterisco de campo obligatorio |
| Gradiente `linear-gradient(270deg, #820933 27%, #D4E79E3B 18%)` | Fondo de la banda de ofertas |

### Contraste WCAG de las combinaciones principales

| Texto / fondo | Ratio | AA texto normal (4,5) | AA texto grande (3) | Dónde |
|---|---|---|---|---|
| `#767522` / `#FFFFFF` | 4,84:1 | Sí, justo | Sí | Logo, nav activo, lista de servicios |
| `#FFFFFF` / `#767522` | 4,84:1 | Sí, justo | Sí | Todo el pie |
| `#820933` / `#FFFFFF` | 10,31:1 | Sí | Sí | Menú |
| `#FFFFFF` / `#820933` | 10,31:1 | Sí | Sí | Botón «Obtener presupuesto» |
| `#D4E79E` / `#820933` | 7,72:1 | Sí | Sí | Texto de ofertas |
| `#000000` / `#D4E79E` | 15,72:1 | Sí | Sí | Testimonios, botón «Contactar» |
| `#820933` / `#D4E79E` | 7,72:1 | Sí | Sí | Autor del testimonio, botón «Enviar» |
| `#D4E79E` / `#767522` | 3,62:1 | **No** | Sí | H1 de Sobre nosotros |
| `#767522` / `#D4E79E` | 3,62:1 | **No** | Sí | H2 «Consúltenos…» (grande, aprueba) y antetítulo de Contacto «Estamos encantados de ayudarte» (16 px; 12 px en móvil; **falla**) |
| `#FFAB00` / `#767522` | 2,55:1 | **No** | **No** | Corchetes del pie y hover de los enlaces del pie |
| `#A3A3A3` / `#FFFFFF` | 2,52:1 | **No** | **No** | Descripción de las tarjetas de oferta (14 px) |
| `#878991` / `#F6F7FA` | 3,26:1 | **No** | Sí | Placeholders, que hacen de etiqueta en el formulario de la home |
| `#757575` / `#FFFFFF` | 4,61:1 | Sí, justo | Sí | Subtítulo de Contacto |
| `#333333` / `#FFFFFF` | 12,63:1 | Sí | Sí | Cuerpo |
| `#D4E79E` / foto + overlay (zona media del hero, muestreada ≈ `#7E6429`) | ≈ 4,2:1 | No, pero es texto grande | Sí | H2 del hero (50 px) |
| `#FFFFFF` / foto + overlay del hero | ≈ 5,6:1 | Sí | Sí | Subtítulo del hero |

Lectura: el oliva sobre blanco aprueba por muy poco. La pareja oliva-lima (3,62:1) solo vale para títulos grandes. El gris de las tarjetas y el ámbar del pie suspenden.

## Tipografías

### Declaradas en los globales de Elementor
- Primary: **Quicksand** 600
- Secondary: **Mulish** 400
- Text: **Mulish** 400
- Accent: **Verdana** 500 (fuente del sistema)

### Cargadas de verdad (`document.fonts`, estado *loaded*)
- **Google Fonts**, enlazadas desde `fonts.googleapis.com`, sin alojar en el propio servidor:
  - Quicksand 600/700
  - Mulish 400/500/700
  - Nunito 400/800
  - Nunito Sans 400 normal e itálica
  - Roboto 400/500
  - IBM Plex Sans 400/500
- **Iconos:** Font Awesome 5 Free (solid y regular), `jkiticon` (Jeg Kit, 392 KB en woff2), eicons y dashicons.
- Elementor pide a Google **todos los pesos del 100 al 900, con itálicas**, de 5 familias en una sola petición, más IBM Plex Sans en otra.

### Uso real por elemento (calculado)

| Elemento | Familia | Tamaño / interlineado | Peso |
|---|---|---|---|
| Cuerpo (`body`) | Pila del sistema (`-apple-system, system-ui, Segoe UI, Roboto…`) del tema Hello | 16/24 px, `#333` | 400 |
| Logo de texto (H2 de cabecera) | Pila del sistema | 32 px | 500 |
| Menú | Verdana | 14 px | 700 |
| Titular del hero (H2) | Quicksand | 50/61 px (33 px en móvil) | 700 |
| Subtítulo del hero (H2) | Mulish | 24/35 px (18 px en móvil) | 500 |
| Títulos de sección (H2/H3 «Más de 60 años…», «NUESTROS SERVICIOS», «Porfolio», «Que opina…») | Quicksand | 35/61 px | 700 |
| H2 del CTA «Te asesoramos sin compromiso» | Roboto | 60/70 px (48 en tablet, 40 en móvil) | 500 |
| H1 de Sobre nosotros | Pila del sistema | 40/40 px | 500 |
| H2 de Sobre nosotros («Te hacemos la vida más fácil», «Consúltenos…») | Verdana | 32 px | 800 / 700 |
| H2 «Contacta con nosotros» | Roboto | 48 px (3rem) | 500 |
| Ventajas (H3) | Mulish | 23 px | 700 |
| Testimonios | Nunito Sans itálica | 17,6/29,9 px | 400 |
| Pie | Nunito | 16/27 px (13 px en móvil) | 400; títulos en 800 con tracking de 4 px |
| Formularios | IBM Plex Sans (campos y textos de MetForm), botón en Roboto | 16 px; botón 14 px | 400-700 |
| Descripción de las tarjetas de oferta | «Muli», que **no se carga** y cae a sans-serif genérica | 14 px | 400 |

**Diagnóstico tipográfico:** en la web conviven **9 familias**: Quicksand, Mulish, Nunito, Nunito Sans, Roboto, IBM Plex Sans, Verdana, la pila del sistema y la fallback de «Muli». Ninguna es una decisión de marca; son restos de plantillas, y los mismos tipos de título usan una familia distinta según la página.

## Tono de voz (rasgos con ejemplo literal)

1. **Directo y descriptivo, de comercio de barrio que dice qué hace y dónde.** «VENTA, INSTALACIÓN Y REPARACIÓN DE TOLDOS Y PERSIANAS EN VALENCIA».
2. **Cercano y familiar, con el cliente en el centro.** «Nos basamos en un trato familiar y personalizado, donde el cliente es nuestra prioridad y queremos que esté satisfecho con los resultados.»
3. **Tranquilizador y sin presión comercial.** «Te asesoramos sin compromiso» / «Contacta con nosotros sin compromiso y nos pondremos en contacto con usted lo antes posible.»
4. **La trayectoria como argumento principal.** «Expertos en toldos y persianas desde 1963» / «Más de 60 años de experiencia».
5. **Práctico y orientado a precio y plazo.** «MAMPARA FIJA DUCHA CRISTAL TEMPLADO EN 48H DESDE 190€» / «Buen precio garantizado».

Además, el tratamiento es **inconsistente**: mezcla tú y usted, a veces en la misma página. Por ejemplo, «Te ayudaremos a elegir el toldo que necesitas» frente a «Consúltenos y le ofreceremos soluciones personalizadas a su medida.» Las mayúsculas sostenidas se usan para dar énfasis.
