# Guía de Uso — SEO Machine Adaptado (Betwinner Argentina)

Esta guía explica cómo usar las nuevas herramientas para optimizar tu sitio de afiliados y suplementos.

## 🚀 Comandos Principales

### 1. Investigación de MercadoLocal
`/research [tema o keyword]`
- **Qué hace**: Busca en Google (vía Serper.dev) con enfoque en **Argentina** y **Villa Carlos Paz**.
- **Resultado**: Crea un brief en `seomachine/research/` con keywords, competencia y estructura recomendada.

### 2. Generación de Borradores
`/draft [tema]`
- **Qué hace**: Crea un artículo SEO-optimizado siguiendo tu **Brand Voice** (Argentino/Voseo) y las directrices de suplementos.
- **Resultado**: Un archivo `.md` listo para revisar.

### 3. Publicación Estática (NUEVO)
`claudecms publish-static <archivo_draft.md>`
- **Qué hace**: Convierte tu borrador Markdown en una página HTML con el mismo diseño premium de tu `index.html`.
- **Resultado**: Crea un archivo `.html` en la carpeta `blog/`.

---

## 🛠️ Configuración Técnica Realizada

1. **API de Serper.dev**: Reemplaza a DataForSEO (más rápido y económico para nosotros).
2. **Google Integration**: Conectado a tu GSC (`sc-domain:bwacceso.com.ar`) y GA4 (`527272226`).
3. **Contexto de Negocio**:
   - `brand-voice.md`: Configurado para hablarle al público argentino ("vos", MercadoPago, etc.).
   - `target-keywords.md`: Lista inicial de keywords de Betwinner y suplementos.
   - `seo-guidelines.md`: Reglas específicas para Cloudflare Pages y Argentina.

## 📁 Archivos Clave
- `seomachine/.env`: Contiene tus llaves (NO compartir).
- `seomachine/google-credentials.json`: Tu acceso a Google APIs.
- `seomachine/test_setup.py`: Ejecutalo si sentís que algo no conecta.

---
**Nota de Mahoraga**: El sistema ha sido adaptado con éxito. Se han neutralized las dependencias de WordPress y DataForSEO para un flujo 100% estático y local.
