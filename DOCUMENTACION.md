# Betwinner Argentina — Documentación de Cambios

## Página de Registro con Código Promocional

Landing page para el registro en Betwinner Argentina con el código promocional **ARGENTINA**, desplegada en Cloudflare Pages.

**URL:** [https://bwacceso.com.ar/](https://bwacceso.com.ar/)

---

## ⚠️ Regla de despliegue

> **Cada vez que se implemente una actualización, se debe pushear automáticamente a GitHub** (`git add . && git commit && git push`). El sitio se despliega vía Cloudflare Pages conectado al repositorio, por lo que el push activa el deploy automáticamente.

---

## Historial de Cambios

### 2026-03-02 — Botón Descargar App + Eliminación de retraso en registro

**Archivos modificados:** `index.html`

#### ✅ Botón "Descargar la App"
- Se agregó un botón **"📲 Descargar la App"** debajo del CTA principal ("Ir al registro").
- Estilo: borde dorado (`var(--gold)`), fondo transparente, con efecto hover que ilumina el fondo.
- Link: `https://bwredir.com/1pIm?p=%2Fmobile%2F`
- Se abre en la misma pestaña (sin `target="_blank"`), igual que el botón de registro.

#### ✅ Eliminación del retraso al registrarse
- Anteriormente, al hacer clic en "Ir al registro", se mostraba un modal con un countdown de 4 segundos antes de redirigir.
- Ahora el flujo es **inmediato**: se copia el código promocional y se redirige al instante a la página de registro de Betwinner.
- Se removió el countdown, el texto "Redirigiendo en X segundos..." y los botones "Ir ahora" / "Cancelar" del modal.

---

### Funcionalidades existentes (implementadas previamente)

- **Código promocional ARGENTINA** con botón de copiar y copia automática al hacer clic en "Ir al registro".
- **Bono de bienvenida** de hasta $72.500 ARS destacado visualmente.
- **Video tutorial** de YouTube embebido con instrucciones de registro.
- **FAQ accordion** con 5 preguntas frecuentes.
- **SEO completo**: meta tags, Open Graph, Twitter Card, JSON-LD structured data.
- **Favicon** personalizado de Betwinner.
- **Archivos SEO**: `sitemap.xml` y `robots.txt`.
- **Diseño premium** dark-themed con animaciones, glassmorphism y tipografías Google Fonts (Bebas Neue, DM Sans).

---

### 2026-03-03 21:58 — Maximización SEO para Google Search Console

**Archivos modificados:** `index.html`, `sitemap.xml`

#### ✅ Meta tags ampliados (`index.html`)
- `<html lang>` actualizado de `es` a `es-AR`.
- `<meta name="keywords">` expandido de 8 a ~40 términos: "cómo apostar en Argentina", "cómo retirar dinero Betwinner", "tutorial apuestas Argentina", "apuestas fútbol Argentina", "Betwinner MercadoPago", "bono primer deposito Argentina", etc.
- `<meta name="description">` enriquecida con frases de búsqueda adicionales.
- `<meta name="robots">` ampliado con `max-snippet:-1, max-image-preview:large, max-video-preview:-1`.
- Nuevos meta tags: `revisit-after`, `language`, `rating`, `classification`, `category`, `coverage`, `distribution`, `target`, `HandheldFriendly`, `MobileOptimized`, `theme-color`, `msapplication-TileColor`.

#### ✅ Geo Targeting
- `geo.region` = AR, `geo.country` = Argentina, `geo.placename` = Argentina, `ICBM` con coordenadas de Buenos Aires, `DC.title`.

#### ✅ Hreflang
- `hreflang="es-ar"`, `hreflang="es"` y `hreflang="x-default"` para señalizar idioma/región a Google.

#### ✅ Open Graph y Twitter Card mejorados
- OG: agregado `og:image:alt`, `og:updated_time`, descripción más rica.
- Twitter: agregado `twitter:image:alt`, `twitter:site`, `twitter:creator`.

#### ✅ Preconnect / DNS-Prefetch
- `preconnect` a Google Fonts y YouTube. `dns-prefetch` a bwredir.com y google-analytics.com.

#### ✅ JSON-LD Structured Data — 5 schemas separados (nuevo)
- **WebPage**: enriquecido con `datePublished`, `dateModified`, `isPartOf (WebSite)`, imagen y publisher con logo.
- **Organization** (nuevo): con `areaServed: Argentina` y `contactPoint`.
- **BreadcrumbList** (nuevo): navegación estructurada para Google.
- **VideoObject** (nuevo): schema para el tutorial de YouTube con `thumbnailUrl`, `embedUrl`, `contentUrl`.
- **FAQPage** (nuevo, separado): 10 preguntas/respuestas sobre depósitos, retiros, MercadoPago, legalidad, app y fútbol argentino.

#### ✅ FAQ visible en HTML expandida
- De 5 a 10 preguntas visibles: métodos de depósito, monto del bono, confiabilidad, fútbol argentino y app móvil.

#### ✅ `sitemap.xml` actualizado
- `lastmod` → `2026-03-03`, `changefreq` → `weekly`.
- Agregados namespace de imagen y video de Google Sitemaps.
- Bloque `<image:image>` con la og-image y bloque `<video:video>` con el tutorial de YouTube.

