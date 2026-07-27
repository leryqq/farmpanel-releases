# Instalación de FarmPanel

**Guía de instalación paso a paso para Windows**

Versión del documento: 1.0

🌐 [English](INSTALL-GUIDE.md) · [Русский](INSTALL-GUIDE.ru.md) · **Español** · [Português](INSTALL-GUIDE.pt.md) · [Français](INSTALL-GUIDE.fr.md) · [Türkçe](INSTALL-GUIDE.tr.md) · [Bahasa Indonesia](INSTALL-GUIDE.id.md) · [Tiếng Việt](INSTALL-GUIDE.vi.md) · [हिन्दी](INSTALL-GUIDE.hi.md) · [中文](INSTALL-GUIDE.zh.md) · [العربية](INSTALL-GUIDE.ar.md)

---

Esta guía te lleva desde la descarga del programa hasta el primer inicio. Sigue los pasos en orden: nada complicado, solo lleva unos minutos.

> **En resumen.** Descarga `Setup.exe` → ejecútalo → activa tu licencia con la clave → listo. No hacen falta permisos de administrador ni instalar nada más por separado.

## Contenido

1. [Qué necesitas](#1-qué-necesitas)
2. [Requisitos del sistema](#2-requisitos-del-sistema)
3. [Paso 1. Descarga el instalador](#paso-1-descarga-el-instalador)
4. [Paso 2. Ejecuta la instalación](#paso-2-ejecuta-la-instalación)
5. [Paso 3. Abre la aplicación](#paso-3-abre-la-aplicación)
6. [Paso 4. Configuración inicial: ubicación de Steam y Sandboxie](#paso-4-configuración-inicial-ubicación-de-steam-y-sandboxie)
7. [Paso 5. Activa tu licencia](#paso-5-activa-tu-licencia)
8. [Paso 6. Comprueba que todo funciona](#paso-6-comprueba-que-todo-funciona)
9. [Actualizaciones](#actualizaciones)
10. [Cómo desinstalar](#cómo-desinstalar)
11. [Solución de problemas de instalación](#solución-de-problemas-de-instalación)
12. [Preguntas frecuentes](#preguntas-frecuentes)

---

# 1. Qué necesitas

- **Un ordenador con Windows 10 u 11** (64 bits).
- **Conexión a internet** — para descargar el programa y activar la licencia.
- **Una clave de licencia** — la recibes con tu compra. Tiene este aspecto:
  `XXXX-XXXX-XXXX-XXXX-XXXX` (cinco grupos de cuatro caracteres).
- **Unos 10 minutos de tu tiempo.**

> **No necesitas** instalar nada más por separado (como .NET): todo lo necesario ya viene incluido en el instalador.

---

# 2. Requisitos del sistema

| Elemento | Mínimo | Recomendado |
|---|---|---|
| Sistema operativo | Windows 10 u 11 (64 bits) | Windows 10 / 11 (64 bits) |
| Memoria | 8 GB | 32 GB |
| Disco | Cualquiera | SSD |
| Espacio libre | unos 500 MB | 1 GB o más |
| Cuentas simultáneas | 2 | 4–10 cuentas de CS2 |
| Resolución de pantalla | al menos 1280 píxeles de ancho | Full HD (1920×1080) o superior |

Si tu ordenador cumple el mínimo, la aplicación funcionará. Cuanto más potente sea el ordenador, más cuentas podrás mantener en marcha a la vez.

---

# Paso 1. Descarga el instalador

1. Abre la página de descargas oficial:
   **[Descargar para Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   (también puedes encontrar el enlace de descarga en el sitio [farmpanel.cc](https://farmpanel.cc)).
2. Busca el archivo con un nombre similar a **`Setup.exe`** (en la sección **Assets**, si estás en la página de versiones) y haz clic para descargarlo.
3. Espera a que termine la descarga. El archivo pesa unos 50–80 MB, así que con una conexión rápida tarda menos de un minuto.

**Qué ocurre después.** El archivo `Setup.exe` aparece en tu carpeta **Descargas** (Downloads).

> **Consejo.** Descarga el instalador solo desde la página oficial enlazada arriba. Así obtienes la versión auténtica y verificada del programa.

![la página de descargas con el archivo Setup.exe](../images/install-download-page.png)

---

# Paso 2. Ejecuta la instalación

1. Abre tu carpeta **Descargas** y haz doble clic en el archivo **`Setup.exe`**.
2. La instalación comienza automáticamente. **No se requieren permisos de administrador**: la aplicación se instala solo para tu cuenta de usuario.
3. Espera a que termine. Suele tardar menos de un minuto. No hay botones «Siguiente» que pulsar: el instalador lo hace todo solo.

**Qué ocurre después.** La aplicación se instala y aparece un icono de **FarmPanel** en el escritorio y en el menú Inicio. A menudo la aplicación se abre justo después de la instalación.

> **Si aparece una ventana azul «Windows protegió tu PC» (SmartScreen)** — es un aviso habitual para programas nuevos, no un error. Qué hacer:
> 1. Pulsa **Más información** (More info).
> 2. Pulsa el botón **Ejecutar de todas formas** (Run anyway) que aparece.
>
> La instalación continúa con normalidad. Más detalles en [Solución de problemas de instalación](#solución-de-problemas-de-instalación).

---

# Paso 3. Abre la aplicación

Si la aplicación no se abrió sola, haz doble clic en el icono de **FarmPanel** del escritorio o búscalo en el menú Inicio.

**Qué verás.** En el primer inicio, la aplicación te guía por una breve configuración inicial y la activación de la licencia: son los pasos siguientes.

---

# Paso 4. Configuración inicial: ubicación de Steam y Sandboxie

En el primer inicio, la aplicación te pide indicar dónde están **Steam** y **Sandboxie-Plus** en tu ordenador. Sin estas rutas, la aplicación no puede iniciar ni aislar las cuentas.

> **Importante.** Para este momento, Sandboxie-Plus ya debe estar instalado. Si aún no lo has hecho, consulta la guía aparte [Instalación de Sandboxie-Plus](../install-sandboxie-plus/INSTALL-SANDBOXIE-PLUS.es.md).

1. **Ubicación de Steam.** Pulsa el botón de selección de carpeta (**Browse…** / icono de carpeta) junto al campo Steam y elige la carpeta donde está instalado Steam. Suele ser `C:\Program Files (x86)\Steam`.
2. **Ubicación de Sandboxie.** Pulsa el botón de selección de carpeta junto al campo Sandboxie y elige la carpeta donde está instalado Sandboxie-Plus. Suele ser `C:\Program Files\Sandboxie-Plus`.
3. Confirma la configuración (el botón **Save** / **Continue**).

**Qué ocurre después.** La aplicación recuerda estas rutas y las usa cada vez que inicia cuentas.

**Señal de éxito.** Ambas rutas están indicadas y la aplicación no muestra avisos de que no encuentra Steam o Sandboxie.

> **Consejo.** Puedes cambiar estas rutas más tarde en cualquier momento en **Settings** (Ajustes).

![configuración inicial: ubicación de Steam y Sandboxie](../images/initial-setup-locations.png)

---

# Paso 5. Activa tu licencia

La activación solo se hace una vez, en el primer inicio.

1. Escribe o pega tu clave de licencia en el campo de entrada.
   Para pegarla desde el portapapeles, pulsa **Paste from clipboard** (Pegar del portapapeles).
2. La aplicación comprueba el formato de la clave mientras escribes. Cuando el formato es correcto, el botón de activación se habilita.
3. Pulsa **Activate** (Activar).

**Qué ocurre después.** La aplicación contacta con el servidor y verifica la clave. Esto tarda unos segundos; verás el estado **Activating** (Activando).

**Señal de éxito.** La ventana de activación se cierra y se abre la pantalla principal de la aplicación: **Dashboard**. Tu licencia está activada. No tendrás que volver a introducir la clave en inicios posteriores.

> **Si la clave no se acepta** — comprueba que la has introducido sin erratas (es más fácil pegarla con **Paste from clipboard**) y que tienes internet. Los mensajes frecuentes se tratan en [Solución de problemas de instalación](#solución-de-problemas-de-instalación).

![la ventana de activación de la licencia](../images/license-activation.png)

---

# Paso 6. Comprueba que todo funciona

Tras la activación llegas a la pantalla principal. Confirma que la instalación tuvo éxito:

1. En la parte superior de la ventana se ve la **barra lateral** con secciones (**Dashboard**, **Accounts**, **Workflows** y otras).
2. En la parte inferior de la ventana está la **barra de estado**: una franja fina con un resumen y la versión de la aplicación (por ejemplo, `v1.0.1`).
3. La aplicación se abre y cambia entre secciones sin errores.

Si todo esto está en su sitio, **la instalación ha terminado y ya puedes usar la aplicación**.

**Qué sigue.** Añade tus cuentas de Steam e inicia tu primera granja. Para instrucciones paso a paso, consulta la [Guía de usuario](../user-guide/USER-GUIDE.es.md) (la sección «Flujos de trabajo principales»).

![la pantalla principal tras la instalación](../images/dashboard-overview.png)

---

# Actualizaciones

FarmPanel se actualiza **automáticamente**: no necesitas descargar nada a mano.

- La aplicación busca nuevas versiones al iniciarse y de vez en cuando mientras funciona.
- La nueva versión se descarga en silencio, en segundo plano, sin interrumpir tu trabajo.
- La actualización se aplica la próxima vez que reinicies la aplicación.

**Qué haces tú.** Nada especial. Basta con cerrar y volver a abrir la aplicación de vez en cuando, y se instalará la última versión. La versión actual siempre se ve en la barra de estado inferior y en **Settings → About**.

---

# Cómo desinstalar

Si necesitas quitar FarmPanel:

1. Abre **Configuración de Windows** → **Aplicaciones** → **Aplicaciones instaladas**
   (o «Panel de control» → «Programas y características»).
2. Busca **FarmPanel** en la lista.
3. Pulsa **Desinstalar** y confirma.

**Qué ocurre después.** La aplicación se elimina de tu ordenador. No hacen falta permisos de administrador para desinstalar.

---

# Solución de problemas de instalación

A continuación tienes situaciones frecuentes y qué hacer en cada caso.

## Apareció una ventana «Windows protegió tu PC» (SmartScreen)

**Causa.** Windows muestra este aviso para programas descargados hace poco y que aún no son muy conocidos por el sistema. No significa que el archivo tenga nada malo.

**Solución.**
1. Pulsa **Más información** (More info).
2. Pulsa **Ejecutar de todas formas** (Run anyway).

La instalación continúa. Si no hay botón **Más información**, asegúrate de haber descargado el archivo desde la página oficial e inténtalo de nuevo.

## Un antivirus bloqueó o eliminó el archivo

**Causa.** Algunos antivirus tratan con cautela los instaladores nuevos y pueden dar una falsa alarma.

**Solución.**
1. Asegúrate de haber descargado `Setup.exe` desde la página oficial (el enlace está en el [Paso 1](#paso-1-descarga-el-instalador)).
2. Si hace falta, añade el archivo a las excepciones del antivirus y descárgalo de nuevo.
3. Si tienes dudas, contacta con soporte (ver [Preguntas frecuentes](#preguntas-frecuentes)).

## El navegador no deja descargar el archivo

**Causa.** El navegador también puede ser cauto al descargar un `.exe`.

**Solución.** En el panel de descargas del navegador, elige **Conservar** (Keep) junto al archivo. Después terminará de descargarse.

## El instalador no se inicia al hacer doble clic

**Solución.**
- Asegúrate de que el archivo se descargó por completo (unos 50–80 MB).
- Haz clic derecho en el archivo y elige **Abrir**.
- Vuelve a descargar el instalador si el archivo está dañado.

## La clave de licencia no se acepta

| Mensaje | Qué significa | Qué hacer |
|---|---|---|
| «License key invalid» | La clave se introdujo con una errata | Comprueba la ortografía. Es más fácil pegar la clave con **Paste from clipboard** |
| «Used on max devices» | La licencia ya se usa en el número máximo de dispositivos | Libera la licencia en otro dispositivo y vuelve a intentarlo. El botón **Manage devices** lleva a la gestión de dispositivos |
| «Cannot reach license server» | No hay conexión con el servidor | Comprueba tu conexión a internet y pulsa **Retry** |

## La aplicación no se abre tras la instalación

**Solución.**
- Ábrela manualmente: el icono de **FarmPanel** en el escritorio o en el menú Inicio.
- Reinicia el ordenador e inténtalo de nuevo.
- Si no ayuda, reinstala la aplicación: desinstálala (ver [Cómo desinstalar](#cómo-desinstalar)) e instálala de nuevo.

---

# Preguntas frecuentes

**¿Necesito permisos de administrador para instalar?**
No. FarmPanel se instala solo para tu cuenta de usuario y no requiere permisos de administrador.

**¿Hace falta instalar .NET u otros componentes por separado?**
No. Todo lo necesario ya viene incluido en el instalador: solo ejecuta `Setup.exe`.

**¿Dónde se instala la aplicación?**
En tu carpeta personal de usuario. No tienes que elegir carpeta manualmente: el instalador se encarga.

**¿Es seguro pulsar «Ejecutar de todas formas» en la ventana de SmartScreen?**
Sí, si descargaste `Setup.exe` desde la página oficial indicada en esta guía. El aviso aparece simplemente porque el programa es nuevo para el sistema.

**¿Dónde se guardan mis contraseñas tras la instalación?**
Solo en tu ordenador. Se cifran con la protección integrada de Windows, nunca se guardan en texto plano y nunca se envían a ningún sitio.

**¿Hay que introducir la clave de licencia cada vez?**
No. La clave se introduce una sola vez, en la primera activación. Después la aplicación se abre directamente en la pantalla principal.

**¿Cómo actualizo la aplicación a una nueva versión?**
No hay que hacer nada: FarmPanel se actualiza automáticamente. Basta con reiniciar la aplicación de vez en cuando para que se instale la última versión (ver [Actualizaciones](#actualizaciones)).

**¿Dónde acudo si algo no funcionó?**
Contacta con soporte en Telegram: [t.me/farmpanel_es](https://t.me/farmpanel_es). Describe el problema y, si tienes uno, incluye el texto del mensaje de error.

---

Tras la instalación, pasa a la [Guía de usuario](../user-guide/USER-GUIDE.es.md): explica en detalle cómo añadir cuentas, iniciarlas y trabajar con la aplicación.

*Fin de la guía de instalación de FarmPanel.*
