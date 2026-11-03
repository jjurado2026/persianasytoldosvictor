# Inventario de imágenes — persianasytoldosvictor.es

- **Origen y tamaño:** se descargó siempre la versión más grande disponible. En los fondos `-scaled` de 2560 px existía el original sin escalar en el servidor, y es el que se guarda. En las miniaturas recortadas de Elementor (`uploads/elementor/thumbs/…`) se guarda el original de 960×960.
- **Medidas:** dimensiones con `sips`; peso del archivo descargado.
- **Carpeta:** todo en `assets/originales/`.
- **Iconos:** van en fuentes de iconos (Font Awesome y jkiticon), no en imágenes, así que no se descargan.

**Resumen:**
- **15 imágenes de contenido únicas**, con 17 usos en la web y 16 archivos descargados (la que se repite se guarda con los dos nombres). Además, 2 grafismos decorativos y el favicon por defecto de WP.
- **8 imágenes únicas reales del cliente**, con 9 usos: toda la galería del porfolio y las 2 tarjetas de oferta (`porfolio-05` y la oferta del toldo son el mismo archivo).
- **7 de stock** (Unsplash y Envato Elements): todos los fondos de hero y CTA y las fotos de ambientación. La de la terraza se usa en la home y en Sobre nosotros.
- **Para una web premium a 1440 px**, solo el stock da resolución. Las fotos reales son de móvil a 960×960, recomprimidas y sin EXIF, probablemente bajadas de Facebook, Instagram o WhatsApp. Sirven a tamaño de tarjeta (hasta unos 480 px de ancho, o 640 con tratamiento), nunca a sangre.

## Imágenes usadas en la web

| Archivo | Página · bloque | Alt en la web | Px (original) | Peso | Origen | Calidad para premium a 1440 px |
|---|---|---|---|---|---|---|
| `home-01-hero-fondo-ventana-stock-unsplash.jpg` (`omar-sotillo-franco-…-unsplash`) | Home · 1 Hero (fondo CSS) | — (fondo) | 5892×3928 | 4,2 MB | **Stock Unsplash** | Resolución sobrada y nítida. Fachada de madera amarilla con un toldo de rayas rojas y blancas: estética nórdica de postal, nada valenciana ni del cliente. En móvil, el recorte solo deja la pared amarilla. Válida técnicamente, pero no es su trabajo. |
| `home-02-experiencia-salon-stock-unsplash.jpg` (`sara-sadeghloo-…-unsplash`) | Home · 2 Experiencia; Sobre nosotros · 2 | vacío (home) / «sara-sadeghloo-A8bjSrQg9CQ-unsplash» (sobre) | 3264×2448 | 1,7 MB | **Stock Unsplash** | Nítida y con buena luz: terraza de hotel bajo una pérgola de lona beige. Sirve a 1440 px, pero es genérica y no muestra un trabajo suyo. |
| `home-03-oferta-toldo-stor-balcon.jpg` (`persianas-toldos-victor-12`) | Home · 3 Ofertas (tarjeta 1) y 8 Galería (foto 5) | «persianas-toldos-victor-12» | 960×960 | 120 KB | **Real del cliente** | Toldo blanco recién instalado en un balcón, desde dentro. Foto de móvil con la cabeza de una persona cortada en primer plano y contraluz. Solo para tarjeta pequeña, y mejor recortada. |
| `home-03-oferta-mampara-ducha.jpg` (`2022-12-14`) | Home · 3 Ofertas (tarjeta 2) | «2022-12-14» | 1280×1280 | 52 KB | **Real del cliente** | Mampara fija en un baño blanco, con el inodoro asomando. 1280 px pero muy comprimida (52 KB): plana y con artefactos. Solo tarjeta pequeña. |
| `home-04-servicios-persianas.png` (`persianas.png`) | Home · 4 Servicios | vacío | 460×310 | 272 KB | **Stock** (por estética: modelo con camisa blanca, luz de estudio) | Muy pequeña (460 px) y en PNG para una foto, con lo que pesa 5 veces más de lo necesario. No sirve a 1440 px. |
| `home-05-cta-fondo-stock-unsplash.jpg` (`rooted-studio-…-unsplash`) | Home · 5 CTA (fondo CSS fijo) | — (fondo) | 6240×4160 | 2,4 MB | **Stock Unsplash** | Toldo azul de un comercio contra el cielo. Nítida, pero con el overlay al 75 % no se ve. Genérica. |
| `home-07-porfolio-01.jpg` (`persianas-toldos-victor-4`) | Home · 8 Galería (grande, fila A) | «persianas-toldos-victor-4» | 960×960 | 184 KB | **Real del cliente** | Toldo con estampado de palmeras en una terraza, con escalera y celosía. Encuadre torcido y caótico; luz dura. Tarjeta. |
| `home-07-porfolio-02.jpg` (`persianas-toldos-victor-2`) | Home · 8 Galería | «persianas-toldos-victor-2» | 960×960 | 96 KB | **Real del cliente** | Cerramiento de lona burdeos con ventanas de cristal en la terraza de un bar, a pie de calle. Es la más «de trabajo terminado»; luz correcta. Tarjeta media. |
| `home-07-porfolio-03.jpg` (`persianas-toldos-victor-9`) | Home · 8 Galería | «persianas-toldos-victor-9» | 960×960 | 71 KB | **Real del cliente** | Interior del mismo cerramiento, de noche, con coches aparcados detrás. Ruido y dominante rojiza. Tarjeta pequeña. |
| `home-07-porfolio-04.jpg` (`persianas-toldos-victor-11`) | Home · 8 Galería | «persianas-toldos-victor-11» | 960×960 | 42 KB | **Real del cliente** | Ventana corredera con persiana nueva, con las pegatinas del fabricante aún puestas y la pared sin pintar alrededor. Muy comprimida. Útil como «antes de terminar»; no como imagen de marca. |
| `home-07-porfolio-05.jpg` | Home · 8 Galería | «persianas-toldos-victor-12» | 960×960 | 120 KB | **Real del cliente** | **Es el mismo archivo que `home-03-oferta-toldo-stor-balcon.jpg`** (mismo md5). Se usa dos veces en la home. |
| `home-07-porfolio-06.jpg` (`persianas-toldos-victor-5`) | Home · 8 Galería | «persianas-toldos-victor-5» | 960×960 | 180 KB | **Real del cliente** | Puertas de celosía marrón y toldo verde en un patio de bajo. Obra a medio recoger (herramientas). Tarjeta. |
| `home-07-porfolio-07.jpg` (`persianas-toldos-victor-`) | Home · 8 Galería (grande, fila B) | «persianas-toldos-victor-&» | 960×960 | 59 KB | **Real del cliente** | Toldos amarillos en una terraza con plantas, desde dentro. Color agradable; poca nitidez. Tarjeta. |
| `sobre-01-hero-persianas-balcon-stock-envato.jpg` (`roller-blinds-on-balcony-windows-…-utc`) | Sobre nosotros · 1 Hero (fondo CSS de columna) | — (fondo) | 3648×5472 | 8,6 MB | **Stock Envato Elements** (sufijo `-utc`) | Estores noche y día en una habitación blanca, con luz rayada. Nítida y muy fotogénica. El original pesa 8,6 MB; la web sirve la versión de 2560. |
| `sobre-01-hero-tarjeta-stock-unsplash.jpg` (`victoire-joncheray-…-unsplash`) | Sobre nosotros · 1 Hero (fondo CSS) | — (fondo) | 5472×3648 | 2,5 MB | **Stock Unsplash** | Fachada con toldos naranjas vista desde abajo. Gráfica y potente. Sirve a 1440 px, pero es genérica. |
| `sobre-03-cta-fondo-stock-unsplash.jpg` (`adam-birkett-…-unsplash`) | Sobre nosotros · 3 CTA (fondo CSS) | — (fondo) | 4000×6000 | 680 KB | **Stock Unsplash** | Canto de un toldo de rayas contra el cielo, con destello de lente. Buena resolución y mucho cielo vacío. |

### Decorativos y sistema

| Archivo | Uso | Px | Peso | Valoración |
|---|---|---|---|---|
| `decor-garabato.png` (`graphic-2.png`) | Garabato junto a las imágenes (home · 2; sobre · 2), oculto en móvil | 212×202 | 2 KB | Resto de la plantilla original («handyman»); no aporta. |
| `decor-flecha.png` (`graphic-arrow-2.png`) | Flecha dibujada (home · 3; sobre · 3) | 218×114 | 2 KB | Resto de plantilla. |
| `favicon-wordpress-por-defecto.png` | `/favicon.ico` redirige aquí | 80×80 | 3 KB | **No es de la marca**: el logo gris por defecto de WordPress. |

## Biblioteca de medios sin usar (por la API REST: 78 archivos en total)

- **Unos 55 archivos** son restos de una plantilla de manitas o reformas importada en marzo de 2023: fontaneros, electricistas, operarios con taladro, avatares de testimonios (`testimonial-*.jpg`), `zz-teammember*.jpg`, `signature-*.png`, `placeholder.png`, etc. También hay fotos de Unsplash y Envato de interiores y toldos. Ninguna es del cliente. No se han descargado.
- **`biblioteca-no-usada-toldo-blanco-balcon.jpg`** (`2023/03/2023-02-02.jpg`, 600×450, 54 KB): **real del cliente**. Es el mismo toldo blanco del balcón, desde otro ángulo; seguramente perteneció a una oferta anterior. Es demasiado pequeña: solo vale como referencia.
- El duplicado `2023/03/2022-12-14.jpg` es idéntico a la foto de la mampara (mismo md5).

## Conclusión para el rediseño

- **Material real del cliente:**
  - 8 fotos únicas de trabajos: toldos, cerramientos, celosías, persiana y mampara.
  - Todas de móvil, a 960 px como máximo, recomprimidas, con encuadres casuales y obra sin terminar en algunas.
  - Valen como **testimonio documental** de trabajos reales en una retícula de tarjetas, con tratamiento uniforme (recorte, corrección de color, quizá duotono con la paleta). **No valen para el hero ni para imagen a sangre.**
- **Stock:**
  - Tiene calidad técnica, pero es genérico y estéticamente ajeno a Valencia.
  - En un rediseño 1:1 se respeta porque es suyo, pero no transmite «60 años de oficio».
- **Lo que falta y habría que cubrir:**
  - foto del local o del taller (Calle Lladró y Malli, 12);
  - foto del equipo o del instalador;
  - furgoneta;
  - detalle de producto (lamas, lonas, motores);
  - trabajos con buena luz a más de 2000 px.
- **Cómo cubrirlo:** pedirlo al cliente; generar con Higgsfield **solo** ambientación (nunca presentada como su local, su equipo o sus trabajos); o usar placeholders etiquetados («retrato del fundador en el taller, luz natural», «furgoneta rotulada en calle de Patraix»).
