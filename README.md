# Invitación de boda · Fernanda & Jorge · 26.02.2027

Archivos:
- `index.html` → la invitación
- `panel.html` → tu panel privado de confirmaciones
- `apps-script.gs` → código para la hoja de Google (no se sube a GitHub; se pega en Google)
- `img/` → fotos, texturas y adornos

---

## Paso 1 · Crear la hoja de confirmaciones (10 min, una sola vez)
1. Entra a sheets.google.com y crea una hoja nueva. Llámala **Confirmaciones boda**.
2. Menú **Extensiones → Apps Script**.
3. Borra lo que aparece y pega todo el contenido de `apps-script.gs`.
4. En la línea `const CLAVE = 'CAMBIA-ESTA-CLAVE';` escribe tu palabra secreta (ej. `fer-jorge-2027`). Guarda (ícono de disquete).
5. Botón azul **Implementar → Nueva implementación**.
   - Tipo (engrane): **Aplicación web**
   - Ejecutar como: **Yo**
   - Quién tiene acceso: **Cualquier usuario**
   - **Implementar** → autoriza con tu cuenta de Google (si sale "Google no verificó esta app": *Configuración avanzada → Ir a … (no seguro)*; es tu propio código).
6. Copia la **URL de la aplicación web** (termina en `/exec`).

## Paso 2 · Pegar la URL en dos lugares
- En `index.html`, busca `PEGA_AQUI_LA_URL_DE_APPS_SCRIPT` y reemplázalo por tu URL.
- En `panel.html`, igual.

## Paso 3 · Publicar en GitHub Pages
1. En github.com → **New repository** → nombre `boda` → **Public** → **Create**.
2. **uploading an existing file** → arrastra `index.html`, `panel.html` y la carpeta `img`. → **Commit changes**.
   (No subas `apps-script.gs`: ahí está tu clave.)
3. **Settings → Pages** → Branch `main` / `(root)` → **Save**.
4. En 1–2 min:
   - Invitación: `https://TU-USUARIO.github.io/boda/`
   - Tu panel: `https://TU-USUARIO.github.io/boda/panel.html` (pide tu clave)

## Ver las confirmaciones
- **Panel**: totales de personas, quién sí y quién no, buscador y botón para descargar a Excel.
- También aparecen en tu hoja de Google, en la pestaña **Confirmaciones**.

## Número máximo de personas
En `index.html`, sección `CONFIGURACIÓN` → `maxPersonas` (hoy: 6).

## Cambiar la fecha límite
En `index.html`, sección `CONFIGURACIÓN` → `fechaLimite` (hoy: 12 de febrero de 2027).

## Si cambias el código de Apps Script
**Implementar → Gestionar implementaciones → editar (lápiz) → Versión: Nueva → Implementar.** La URL no cambia.
