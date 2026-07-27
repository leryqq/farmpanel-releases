# Instalación de Sandboxie-Plus

**Guía de instalación paso a paso para Windows**

Versión del documento: 1.0 · Versión de Sandboxie-Plus: **1.17.5**

🌐 [English](INSTALL-SANDBOXIE-PLUS.md) · [Русский](INSTALL-SANDBOXIE-PLUS.ru.md) · **Español** · [Português](INSTALL-SANDBOXIE-PLUS.pt.md) · [Français](INSTALL-SANDBOXIE-PLUS.fr.md) · [Türkçe](INSTALL-SANDBOXIE-PLUS.tr.md) · [Bahasa Indonesia](INSTALL-SANDBOXIE-PLUS.id.md) · [Tiếng Việt](INSTALL-SANDBOXIE-PLUS.vi.md) · [हिन्दी](INSTALL-SANDBOXIE-PLUS.hi.md) · [中文](INSTALL-SANDBOXIE-PLUS.zh.md) · [العربية](INSTALL-SANDBOXIE-PLUS.ar.md)

---

FarmPanel mantiene cada cuenta en su propia **sandbox**: un entorno aislado donde Steam y CS2 no se solapan con otras cuentas. De este aislamiento se encarga un programa gratuito llamado **Sandboxie-Plus**. Se instala una sola vez, antes de empezar a iniciar cuentas en FarmPanel.

Esta guía te acompaña en la instalación paso a paso. Nada complicado: lleva unos minutos.

> **En resumen.** Descarga el instalador de **Sandboxie-Plus 1.17.5** → ejecútalo → acepta la configuración por defecto → permite la instalación (se requieren permisos de administrador) → listo.

> **Importante.** A diferencia de FarmPanel, Sandboxie-Plus **requiere permisos de administrador** para instalarse; es normal, porque el programa se integra en Windows a un nivel profundo para aislar aplicaciones de forma fiable.

## Contenido

1. [Qué necesitas](#1-qué-necesitas)
2. [Paso 1. Descarga el instalador](#paso-1-descarga-el-instalador)
3. [Paso 2. Ejecuta la instalación](#paso-2-ejecuta-la-instalación)
4. [Paso 3. Completa el asistente de instalación](#paso-3-completa-el-asistente-de-instalación)
5. [Paso 4. Primer inicio de Sandboxie-Plus](#paso-4-primer-inicio-de-sandboxie-plus)
6. [Paso 5. Comprueba que todo funciona](#paso-5-comprueba-que-todo-funciona)
7. [Paso 6. Conéctalo con FarmPanel](#paso-6-conéctalo-con-farmpanel)
8. [Cómo desinstalar Sandboxie-Plus](#cómo-desinstalar-sandboxie-plus)
9. [Solución de problemas](#solución-de-problemas)
10. [Preguntas frecuentes](#preguntas-frecuentes)

---

# 1. Qué necesitas

- **Un ordenador con Windows 10 u 11** (64 bits).
- **Permisos de administrador** en este ordenador (durante la instalación aparece un aviso — hay que pulsar **Sí**).
- **Conexión a internet** — para descargar el programa.
- **Unos 5 minutos de tu tiempo.**

> Sandboxie-Plus es gratuito. Algunas funciones adicionales están disponibles para quienes apoyan el proyecto, pero **no las necesitas** para trabajar con FarmPanel: la versión gratuita normal es suficiente.

---

# Paso 1. Descarga el instalador

1. Abre la página oficial de la versión que necesitas:
   **[Sandboxie-Plus 1.17.5 en GitHub](https://github.com/sandboxie-plus/Sandboxie/releases/tag/v1.17.5)**
2. Baja hasta la sección **Assets** (Archivos).
3. Busca y descarga el archivo con un nombre similar a **`Sandboxie-Plus-x64-v1.17.5.exe`** — es el instalador para un Windows normal de 64 bits.

**Cómo elegir el archivo correcto:**

| Archivo | Para quién es |
|---|---|
| **`Sandboxie-Plus-x64-v1.17.5.exe`** | **La mayoría de usuarios** — un Windows normal con procesador Intel o AMD. Descarga este. |
| `Sandboxie-Plus-arm64-v1.17.5.exe` | Solo para ordenadores con procesador ARM (poco frecuente). |
| `Sandboxie-Classic-…` | La variante de interfaz antigua. **No es necesaria** para FarmPanel — elige **Plus**. |
| Archivos `.7z` | Versiones portables para usuarios avanzados. **No son necesarias** para la instalación. |

**Qué ocurre después.** El archivo aparece en tu carpeta **Descargas** (Downloads).

> **Consejo.** Descarga el instalador solo desde la página oficial de GitHub enlazada arriba. Así obtienes la versión auténtica y verificada.

![la página de la versión 1.17.5 con la sección Assets](../images/sandboxie/github-release-assets.png)

---

# Paso 2. Ejecuta la instalación

1. Abre tu carpeta **Descargas** y haz doble clic en el archivo descargado **`Sandboxie-Plus-x64-v1.17.5.exe`**.
2. Windows mostrará el aviso **«¿Quieres permitir que esta aplicación haga cambios en tu dispositivo?»** — pulsa **Sí**. Este es el aviso de permisos de administrador; sin él no se puede instalar Sandboxie-Plus.

> **Si aparece una ventana azul de SmartScreen** («Windows protegió tu PC») — pulsa **Más información**, luego **Ejecutar de todas formas**. Es un aviso habitual para programas descargados, no un error.

**Qué ocurre después.** Se abre la ventana del asistente de instalación.

---

# Paso 3. Completa el asistente de instalación

El asistente de instalación te guía por unas pantallas sencillas. En la mayoría de los casos basta con dejar todo por defecto y pulsar **Next** (Siguiente).

1. **Selección de idioma.** Si aparece una ventana de selección de idioma, elige español (o inglés) y pulsa **OK**.
2. **Acuerdo de licencia.** Léelo y pulsa **I Agree** (Acepto) o **Next**.
3. **Carpeta de instalación.** Deja la carpeta por defecto (`C:\Program Files\Sandboxie-Plus`) y pulsa **Next**. No hace falta cambiarla.
4. **Opciones de instalación.** No hay que cambiar nada — simplemente pulsa **Next** / **Install** (Instalar).
5. Espera a que termine. La instalación tarda menos de un minuto.
6. En la última pantalla, pulsa **Finish** (Finalizar). Deja marcada la casilla de iniciar Sandboxie-Plus, si la hay.

**Qué ocurre después.** Sandboxie-Plus se instala y su icono aparece en el escritorio y en el menú Inicio. El programa suele iniciarse justo después de la instalación.

> **¿Hace falta reiniciar?** Por lo general, no. Pero si el asistente pide reiniciar el ordenador, hazlo para que el aislamiento funcione correctamente.

![la pantalla del asistente de instalación con la carpeta por defecto](../images/sandboxie/installer-wizard.png)

---

# Paso 4. Primer inicio de Sandboxie-Plus

La primera vez que abres Sandboxie-Plus, muestra un **asistente de configuración** (Setup Wizard). Complétalo paso a paso: simplemente repite lo que se describe abajo.

Si antes del asistente aparece una ventana de **selección de idioma de la interfaz**, elige tu idioma y pulsa **OK**.

Después, el asistente te guía por varias pantallas.

### Pantalla 1 — Introduction (Introducción)

Selecciona la opción **«Personally, for private non-commercial use»** (Para uso personal no comercial) y pulsa **Next** (Siguiente).

![Setup Wizard — la pantalla Introduction con «Personally, for private non-commercial use» seleccionado](../images/sandboxie/wizard-1-introduction.png)

### Pantalla 2 — Support certificate (Certificado de apoyo)

Deja el campo **vacío** y pulsa **Next**. No hace falta un certificado para trabajar con FarmPanel.

![Setup Wizard — la pantalla Support certificate con el campo vacío](../images/sandboxie/wizard-2-support-certificate.png)

### Pantalla 3 — Configure UI (Configuración de la interfaz)

Deja los valores **por defecto** (la opción **Advanced UI for experts** ya está seleccionada) y pulsa **Next**.

![Setup Wizard — la pantalla de configuración de la interfaz con los valores por defecto](../images/sandboxie/wizard-3-ui-configuration.png)

### Pantalla 4 — Shell integration (Integración con el sistema)

**Desmarca todas las casillas** y pulsa **Next**.

![Setup Wizard — la pantalla Shell integration con todas las casillas desmarcadas](../images/sandboxie/wizard-4-shell-integration.png)

### Pantalla 5 — Updater (Actualizaciones)

**Desmarca todas las casillas** y pulsa **Next**.

![Setup Wizard — la pantalla Updater con todas las casillas desmarcadas](../images/sandboxie/wizard-5-updater.png)

### Pantalla 6 — Complete (Finalizar)

Pulsa **Finish** (Finalizar) para aplicar la configuración y cerrar el asistente.

![Setup Wizard — la pantalla final con el botón Finish](../images/sandboxie/wizard-6-complete.png)

> **Consejo.** Si dudas en alguna pantalla, desmarca las casillas y pulsa **Next**. FarmPanel no necesita las integraciones adicionales ni los recordatorios de actualización.

**Qué ocurre después.** Se abre la ventana principal de Sandboxie-Plus — la lista de sandboxes y el panel de control.

![la ventana principal de Sandboxie-Plus tras el primer inicio](../images/sandboxie/main-window.png)

---

# Paso 5. Comprueba que todo funciona

Asegúrate de que Sandboxie-Plus está instalado correctamente:

1. Abre Sandboxie-Plus (el icono del escritorio o del menú Inicio).
2. La ventana principal muestra una lista de sandboxes — normalmente ya hay una sandbox por defecto con un nombre como **DefaultBox**.
3. El programa se abre y no muestra mensajes de error.

Si todo esto está en su sitio, **Sandboxie-Plus está instalado y listo para usar**.

---

# Paso 6. Conéctalo con FarmPanel

Una vez instalado Sandboxie-Plus, FarmPanel podrá usarlo para aislar las cuentas.

1. Abre **FarmPanel**.
2. Ve a **Settings → Sandboxes** (Ajustes → Sandboxes).
3. Asegúrate de que la ruta de la carpeta de sandboxes está indicada. Si el campo está vacío, elige una carpeta para las sandboxes; si ya está rellenado, no hay que cambiar nada.
4. Vuelve a la pantalla **Accounts**. Ahora, al añadir cuentas, puedes elegir cómo se asignan las sandboxes (**Auto-assign** y otras), y las cuentas se pueden iniciar.

> **Cómo se conecta.** En FarmPanel, cada cuenta debe estar vinculada a una sandbox; de lo contrario no se puede iniciar. Es Sandboxie-Plus quien crea y mantiene estos entornos aislados «por debajo». Para más información sobre las sandboxes y el inicio de cuentas, consulta la [Guía de usuario de FarmPanel](../user-guide/USER-GUIDE.es.md).

**Señal de éxito.** Una cuenta en FarmPanel se inicia y pasa al estado **Running** (En marcha), lo que significa que el aislamiento a través de Sandboxie-Plus funciona.

---

# Cómo desinstalar Sandboxie-Plus

Si necesitas quitar el programa:

1. Primero, cierra todos los programas que se ejecutan en sandboxes (en FarmPanel, detén las cuentas con **Stop**).
2. Abre **Configuración de Windows** → **Aplicaciones** → **Aplicaciones instaladas**
   (o «Panel de control» → «Programas y características»).
3. Busca **Sandboxie-Plus** en la lista.
4. Pulsa **Desinstalar** y confirma. Para desinstalar también hacen falta permisos de administrador.

> **Ten en cuenta.** Tras quitar Sandboxie-Plus, FarmPanel no podrá iniciar cuentas hasta que el programa se instale de nuevo.

---

# Solución de problemas

## Windows no deja instalar — no hay permisos de administrador

**Causa.** Sandboxie-Plus requiere obligatoriamente permisos de administrador.

**Solución.** Inicia sesión con una cuenta que tenga permisos de administrador, o pide al administrador del ordenador que instale el programa. Cuando aparezca el aviso **«¿Permitir hacer cambios?»**, pulsa **Sí**.

## Apareció una ventana de SmartScreen

**Causa.** Windows avisa sobre programas descargados hace poco. No es un error.

**Solución.** Pulsa **Más información** (More info), luego **Ejecutar de todas formas** (Run anyway).

## Un antivirus bloqueó el instalador

**Causa.** Algunos antivirus tratan con cautela el software que se integra en el sistema.

**Solución.**
1. Asegúrate de haber descargado el archivo desde la página oficial de GitHub (el enlace está en el [Paso 1](#paso-1-descarga-el-instalador)).
2. Si hace falta, añade temporalmente el archivo a las excepciones del antivirus y descárgalo de nuevo.

## Descargaste el archivo equivocado

**Causa.** En la página de la versión hay varios archivos.

**Solución.** Para un Windows normal necesitas el archivo llamado **`Sandboxie-Plus-x64-v1.17.5.exe`**. No tomes las variantes **arm64**, **Classic** ni los archivos **.7z**. Vuelve al [Paso 1](#paso-1-descarga-el-instalador) y descarga el archivo correcto.

## FarmPanel no inicia cuentas tras la instalación

**Solución.**
1. Asegúrate de que Sandboxie-Plus está instalado y se abre (ver [Paso 5](#paso-5-comprueba-que-todo-funciona)).
2. En FarmPanel, abre **Settings → Sandboxes** y comprueba que la ruta de la carpeta de sandboxes está indicada.
3. Reinicia FarmPanel.
4. Si el problema persiste, contacta con soporte (ver [Preguntas frecuentes](#preguntas-frecuentes)).

## El ordenador pide reiniciar tras la instalación

**Solución.** Reinicia el ordenador — esto completa la instalación y activa el aislamiento. Tras reiniciar, abre FarmPanel de nuevo.

---

# Preguntas frecuentes

**¿Es obligatorio instalar Sandboxie-Plus?**
Sí, si quieres iniciar cuentas en FarmPanel. Es Sandboxie-Plus quien proporciona el aislamiento de cada cuenta en un entorno separado.

**¿Sandboxie-Plus es de pago?**
No, la versión básica es gratuita y es suficiente para trabajar con FarmPanel. Hay funciones adicionales para quienes apoyan el proyecto, pero no son necesarias.

**¿Por qué la instalación requiere permisos de administrador y FarmPanel no?**
Sandboxie-Plus se integra en Windows a un nivel profundo para aislar programas de forma fiable, por eso necesita permisos de administrador. FarmPanel, en cambio, se instala solo para tu cuenta de usuario y no los requiere.

**¿Hay que configurar las sandboxes a mano?**
No. Basta con instalar Sandboxie-Plus. FarmPanel crea y configura las sandboxes para las cuentas automáticamente.

**¿Necesito un certificado de apoyo (supporter certificate)?**
No. Puedes omitir esa pantalla en el primer inicio. No es necesario para FarmPanel.

**¿Qué versión exacta debo instalar?**
La versión **1.17.5** — el enlace está en el [Paso 1](#paso-1-descarga-el-instalador). Instala exactamente esa para una compatibilidad predecible con FarmPanel.

**¿Dónde acudo si algo no funcionó?**
Contacta con el soporte de FarmPanel en Telegram: [t.me/farmpanel_es](https://t.me/farmpanel_es). Describe el problema e incluye el texto del mensaje de error si lo tienes.

---

Tras instalar Sandboxie-Plus, vuelve a la [guía de instalación de FarmPanel](../install-guide/INSTALL-GUIDE.es.md) o directamente a la [Guía de usuario](../user-guide/USER-GUIDE.es.md) para añadir cuentas e iniciar tu primera granja.

*Fin de la guía de instalación de Sandboxie-Plus.*
