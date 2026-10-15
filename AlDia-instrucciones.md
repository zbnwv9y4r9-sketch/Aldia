# AlDía

App para anotar los gastos e ingresos del mes, marcar pagos y ver cuánto te queda. Funciona en el navegador y se instala en el celular como una app.

## Qué hay en esta carpeta

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app completa |
| `manifest.json` | Permite instalarla en el celular con nombre e ícono |
| `sw.js` | Hace que abra rápido y funcione sin internet |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` | Íconos |

## Publicarla en GitHub Pages

1. Crea una cuenta gratis en https://github.com si no tienes una.
2. Toca **+** (arriba a la derecha) y luego **New repository**.
3. Nombre: `aldia`. Marca **Public** y toca **Create repository**.
4. En la página del repositorio toca **uploading an existing file** (o **Add file → Upload files**).
5. Arrastra **todos** los archivos de esta carpeta (no la carpeta, sus archivos) y toca **Commit changes**.
6. Ve a **Settings → Pages**. En **Source** elige **Deploy from a branch**, en **Branch** elige `main` y `/ (root)`, y toca **Save**.
7. Espera uno o dos minutos y recarga. Aparecerá tu dirección, parecida a:
   `https://TU-USUARIO.github.io/aldia/`

## Instalarla en el celular

- **iPhone:** abre la dirección en **Safari**, toca **Compartir** y luego **Agregar a pantalla de inicio**.
- **Android:** abre la dirección en **Chrome**, toca el menú **⋮** y luego **Instalar app** (o **Agregar a pantalla principal**).

La primera vez te pedirá crear tu código de entrada.

## Privacidad

- Los datos (gastos, ingresos, código) se guardan **solo en el teléfono de cada persona**. Nunca se suben a GitHub ni a ningún servidor.
- Cada persona que la instale empieza vacía y tiene sus propios datos y su propio código.
- Con una cuenta gratis de GitHub el repositorio debe ser público: cualquiera puede ver el **código** de la app, pero no los datos de nadie.
- Para un repositorio privado con GitHub Pages necesitas un plan de pago de GitHub (Pro o superior).
- Cualquier persona con la dirección puede abrir la app. No hay forma de aprobar quién la instala con GitHub Pages.

## Respaldos

Como los datos viven en el teléfono, si borras el navegador o cambias de teléfono se pierden. En **Historial → Respaldo**:
- **Guardar respaldo** descarga un archivo con tus datos. Guárdalo en tu correo, Drive o iCloud.
- **Cargar respaldo** lo restaura (reemplaza los datos actuales).

El código de entrada no va en el respaldo; en el teléfono nuevo creas uno.

## Actualizar la app

1. Sube el `index.html` nuevo al repositorio (reemplaza el anterior).
2. En `sw.js` cambia `aldia-v1` por `aldia-v2` (y así cada vez) y súbelo también.
3. Cierra y vuelve a abrir la app en el celular; puede tardar una o dos aperturas en mostrar la versión nueva.

## Diferencias con la versión en Claude

- **No incluye la revisión de correos de Gmail.** Eso necesita un servidor propio y permisos de Google; se puede agregar más adelante.
- Los datos no se sincronizan entre teléfonos; usa los respaldos para pasarlos.

## Si olvidas el código de entrada

Borra los datos del sitio en el navegador (en iPhone: Ajustes → Safari → Avanzado → Datos de sitios web; en Android: Chrome → Configuración del sitio). Esto **borra también tus gastos**, así que conviene tener un respaldo reciente.
