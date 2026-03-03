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
