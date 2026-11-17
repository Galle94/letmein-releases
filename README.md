# LetMeIn — descargas e instalación

Aquí se publican las versiones de LetMeIn: la app de escritorio (Windows, macOS y Linux), la app
de Android y la extensión del navegador.

**[⬇ Descargar la última versión](https://github.com/Galle94/letmein-releases/releases/latest)**
(los archivos están en la sección *Assets*, al final de la página del release).

Los instaladores son de uso interno y **no están firmados** por Microsoft, Apple, Google ni
Mozilla. Por eso cada sistema muestra un aviso la primera vez. Es normal; abajo se explica qué
hacer en cada caso.

- [Windows](#windows)
- [macOS](#macos)
- [Linux](#linux)
- [Android](#android)
- [Extensión para Chrome y Edge](#extensión-para-chrome-y-edge)
- [Extensión para Firefox](#extensión-para-firefox)
- [Primer inicio](#primer-inicio)

---

## Windows

**Qué descargar:** `LetMeIn_<versión>_x64-setup.exe` (el `.msi` también sirve).

1. Abre el archivo descargado.
2. Si aparece **«Windows protegió su PC»** (SmartScreen), pulsa **Más información** y después
   **Ejecutar de todas formas**.
3. Sigue el instalador. LetMeIn queda en el menú Inicio.

**Actualizar:** en la app, **Ajustes → Actualizaciones → Buscar actualizaciones**. Descarga e
instala la versión nueva y reinicia la app; no hace falta volver a descargar nada.

## macOS

**Qué descargar:** `LetMeIn_<versión>_universal.dmg` (funciona en Mac con Apple Silicon e Intel).

1. Abre el `.dmg` y arrastra **LetMeIn** a la carpeta **Aplicaciones**.
2. La primera vez, macOS dirá que no puede comprobar el desarrollador. Para abrirla:
   - **macOS 15 (Sequoia) o posterior:** intenta abrir la app, cierra el aviso, ve a
     **Ajustes del Sistema → Privacidad y seguridad**, baja hasta el mensaje sobre LetMeIn y pulsa
     **Abrir igualmente**. Confirma con tu contraseña.
   - **macOS 14 o anterior:** en Aplicaciones, **clic derecho (o Control+clic) sobre LetMeIn →
     Abrir**, y en el aviso pulsa **Abrir**.
3. Si macOS dice que la app **«está dañada»**, abre Terminal y ejecuta:

   ```bash
   xattr -cr /Applications/LetMeIn.app
   ```

   Después ábrela de nuevo.

Solo hay que hacerlo la primera vez.

**Actualizar:** **Ajustes → Actualizaciones → Buscar actualizaciones**, igual que en Windows.

## Linux

**Qué descargar**, según tu distribución:

- **Cualquier distribución:** `LetMeIn_<versión>_amd64.AppImage`. Dale permiso de ejecución y
  ábrelo:

  ```bash
  chmod +x LetMeIn_*_amd64.AppImage
  ./LetMeIn_*_amd64.AppImage
  ```

- **Debian, Ubuntu y derivadas:** `LetMeIn_<versión>_amd64.deb`:

  ```bash
  sudo apt install ./LetMeIn_*_amd64.deb
  ```

- **Fedora y derivadas:** el archivo `.rpm`:

  ```bash
  sudo dnf install ./LetMeIn-*.x86_64.rpm
  ```

**Actualizar:** con el AppImage, desde **Ajustes → Actualizaciones**. Con `.deb` o `.rpm`,
descarga el paquete nuevo e instálalo con el mismo comando.

## Android

**Qué descargar:** `LetMeIn_<versión>_android_arm64.apk` (Android 7 o posterior). Lo más
cómodo es abrir esta página directamente desde el celular.

1. Descarga el APK y ábrelo desde la notificación o desde la app **Archivos**.
2. Android pedirá permiso para **instalar apps desconocidas** desde el navegador (o la app de
   archivos). Pulsa **Configuración**, activa **Permitir de esta fuente** y vuelve atrás.
3. Pulsa **Instalar**.
4. Si **Play Protect** avisa de que la app es desconocida, pulsa **Más detalles → Instalar de
   todas formas**. Si pregunta si quieres enviarla para analizarla, puedes responder que no.

**Actualizar:** en la app, **Ajustes → Actualizaciones → Buscar actualizaciones**. Si hay una
versión nueva se descarga el APK; al abrirlo, Android la instala encima **conservando tus datos**.

> Si alguna vez instalaste una versión de prueba que no venía de esta página, Android no dejará
> instalar encima («la app no está instalada» o «conflicto con un paquete existente»).
> Desinstala la anterior, instala esta y vuelve a entrar con tu correo, contraseña maestra y
> Secret Key.

## Extensión para Chrome y Edge

**Qué descargar:** `LetMeIn_<versión>_extension_chrome.zip`. Sirve también para Edge, Brave y
otros navegadores basados en Chromium.

La extensión no está en la Chrome Web Store, así que se instala en «modo desarrollador»:

1. **Descomprime el zip en una carpeta que no vayas a borrar**, por ejemplo
   `Documentos\LetMeIn-extension`. El navegador la usa desde ahí: si borras la carpeta, la
   extensión deja de funcionar.
2. Abre `chrome://extensions` (en Edge, `edge://extensions`).
3. Activa **Modo de desarrollador** (arriba a la derecha en Chrome; en el menú lateral en Edge).
4. Pulsa **Cargar descomprimida** y elige la carpeta del paso 1 (la que contiene
   `manifest.json`).
5. Fija la extensión: pulsa el icono de la pieza de puzle en la barra y luego la chincheta de
   LetMeIn.
6. Abre la extensión e inicia sesión con la dirección del servidor, tu correo, tu contraseña
   maestra y tu Secret Key.

Es normal que el navegador avise a veces de que hay extensiones en modo desarrollador. Puedes
cerrar el aviso; no la desactives.

**Actualizar:** la extensión no se actualiza sola. Descarga el zip de la versión nueva,
**reemplaza el contenido de la misma carpeta** con el del zip y, en `chrome://extensions`, pulsa
el botón de recargar (↻) de LetMeIn.

**Atajo:** `Ctrl+Shift+L` (`Cmd+Shift+L` en Mac) rellena el formulario de la página si hay una
sola cuenta guardada para ella.

## Extensión para Firefox

**Qué descargar:** `LetMeIn_<versión>_extension_firefox.zip` (Firefox 128 o posterior).

Por ahora la extensión de Firefox no está firmada por Mozilla, así que solo se puede cargar
**de forma temporal: se quita al cerrar Firefox** y hay que volver a cargarla en cada sesión.

1. Descomprime el zip en una carpeta.
2. Abre `about:debugging#/runtime/this-firefox`.
3. Pulsa **Cargar complemento temporal…** y elige el archivo `manifest.json` de esa carpeta.

## Primer inicio

Al abrir la app por primera vez verás tres opciones:

- **Tengo una invitación:** si te invitaron por correo. Abre el enlace del correo en el
  dispositivo donde instalaste LetMeIn, o pega el enlace o el código en la app.
- **Ya tengo cuenta:** para añadir otro dispositivo a tu bóveda. Lo más rápido es, en un
  dispositivo donde ya tengas sesión, ir a **Ajustes → Añadir un dispositivo** y escanear el QR o
  escribir el código que aparece. También puedes entrar con tu correo, tu contraseña maestra y tu
  **Secret Key**.
- **Crear bóveda:** una bóveda nueva y vacía.

**Guarda tu Secret Key** en un lugar seguro cuando la app te la muestre. Junto con tu contraseña
maestra, es lo único que permite abrir tu bóveda en un dispositivo nuevo: nadie puede
recuperarla por ti.
