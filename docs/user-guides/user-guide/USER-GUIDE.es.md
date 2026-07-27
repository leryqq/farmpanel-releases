# Guía de usuario de FarmPanel

**Panel de control para tu granja de cuentas de Steam y CS2 en Windows**

Versión del documento: 1.0

🌐 [English](USER-GUIDE.md) · [Русский](USER-GUIDE.ru.md) · **Español** · [Português](USER-GUIDE.pt.md) · [Français](USER-GUIDE.fr.md) · [Türkçe](USER-GUIDE.tr.md) · [Bahasa Indonesia](USER-GUIDE.id.md) · [Tiếng Việt](USER-GUIDE.vi.md) · [हिन्दी](USER-GUIDE.hi.md) · [中文](USER-GUIDE.zh.md) · [العربية](USER-GUIDE.ar.md)

---

> **Cómo leer esta guía.** Los botones, pestañas y estados aparecen en la aplicación en inglés. Para que siempre pulses lo correcto, los nombres de los elementos de la interfaz se muestran **tal como aparecen en pantalla** (por ejemplo, **Add Account**, **Start**, **Running**), con la explicación en español. La primera vez que se menciona un elemento importante se acompaña de su traducción entre paréntesis.

## Contenido

1. [Introducción](#1-introducción)
2. [Antes de empezar](#2-antes-de-empezar)
3. [Primer inicio](#3-primer-inicio)
4. [Descripción de la interfaz](#4-descripción-de-la-interfaz)
5. [Flujos de trabajo principales](#5-flujos-de-trabajo-principales)
6. [Tareas habituales («Quiero…»)](#6-tareas-habituales-quiero)
7. [Referencia de funciones](#7-referencia-de-funciones)
8. [Estados e indicadores](#8-estados-e-indicadores)
9. [Notificaciones](#9-notificaciones)
10. [Errores y solución de problemas](#10-errores-y-solución-de-problemas)
11. [Buenas prácticas](#11-buenas-prácticas)
12. [Preguntas frecuentes](#12-preguntas-frecuentes)

---

# 1. Introducción

## Qué es FarmPanel

**FarmPanel** es una aplicación de escritorio para Windows que te ayuda a gestionar muchas cuentas de Steam y clientes de Counter-Strike 2 desde una sola ventana. En lugar de abrir a mano decenas de ventanas de Steam, vigilar cada una y reiniciar las que se congelan, gestionas toda tu granja de cuentas de forma centralizada, desde un panel claro.

FarmPanel inicia los clientes, aísla las cuentas entre sí, vigila su estado en tiempo real y las recupera automáticamente tras un fallo.

> **Importante.** FarmPanel **no es un bot ni un auto-farmeo**. No juega por ti ni imita acciones dentro del juego. Gestiona todo lo que ocurre *alrededor* del juego: el inicio de los clientes, las invitaciones a la sala, la recuperación tras fallos y la visibilidad en vivo de cada cuenta. Todas las acciones dentro del juego las realiza una persona real.

## Qué problemas resuelve

Si tienes más de una cuenta, esta rutina te resultará familiar:

- hay que iniciar decenas de clientes de Steam y CS2;
- cada cuenta debe funcionar por separado, sin interferir con las demás;
- crear salas y enviar invitaciones a mano es lento y cansado;
- un CS2 caído hay que detectarlo y reiniciarlo a tiempo;
- es difícil saber quién ya está en una partida y quién se quedó cargando.

FarmPanel elimina esta rutina y reúne todas las operaciones en una sola aplicación.

## Para quién es

La aplicación está pensada para quien necesita gestionar de forma centralizada muchas cuentas de Steam y CS2 —desde unas pocas hasta varios cientos— con inicio automatizado, supervisión en vivo y recuperación fiable tras fallos.

## Qué podrás hacer

- Guardar todas las cuentas en un solo lugar y encontrar rápidamente la que necesitas.
- Iniciar y detener cuentas de una en una o todas a la vez.
- Aislar cada cuenta en su propio entorno protegido (una sandbox).
- Formar grupos (party) de cuentas y ponerlas en cola de emparejamiento juntas.
- Vigilar la carga del equipo, el estado de los procesos y las caídas en tiempo real.
- Recuperar automáticamente las cuentas tras una caída o tras cerrar la aplicación.
- Distribuir las ventanas de CS2 por los monitores según un diseño predefinido.

![pantalla principal de FarmPanel (Dashboard)](../images/dashboard-overview.png)

---

# 2. Antes de empezar

## Requisitos del sistema

| Elemento | Mínimo | Recomendado |
|---|---|---|
| Sistema operativo | Windows 10 u 11 (64 bits) | Windows 10 / 11 (64 bits) |
| Memoria | 8 GB | 32 GB |
| Disco | Cualquiera | SSD |
| Cuentas simultáneas | 2 | 4–10 cuentas de CS2 |
| Resolución de pantalla | Área de trabajo de al menos 1280 píxeles de ancho | Full HD (1920×1080) o superior |

## Qué preparar de antemano

- **El instalador de FarmPanel** — un archivo llamado `Setup.exe` que descargas desde la página de descargas oficial.
- **Una clave de licencia** — la recibes con tu compra. Tiene este aspecto: `XXXX-XXXX-XXXX-XXXX-XXXX` (cinco grupos de cuatro caracteres).
- **Los datos de tus cuentas de Steam** — usuarios y contraseñas, y códigos de Steam Guard si los usas. Puedes introducirlos uno a uno o importar una lista desde un archivo.
- **Conexión a internet** — necesaria en el primer inicio para activar la licencia y, después, para que funcionen Steam y CS2.

## Permisos

- La instalación **no requiere permisos de administrador**: la aplicación se instala solo para tu cuenta de usuario.
- La primera vez que ejecutes el instalador, Windows puede mostrar una ventana azul de **SmartScreen** («Windows protegió tu PC»); es un aviso habitual para programas nuevos. Pulsa **Más información** y luego **Ejecutar de todas formas**.
- La aplicación puede necesitar acceso a la red (para Steam) y a las reglas del Firewall de Windows. Si aparece un aviso del firewall, permite el acceso.

## Dónde se guardan tus datos

Los usuarios y las contraseñas se cifran con la protección integrada de Windows y se guardan **solo en tu equipo**. Nunca se almacenan en texto plano ni se envían a ningún sitio.

---

# 3. Primer inicio

A continuación tienes el recorrido desde la instalación hasta un panel listo para usar. Sigue los pasos en orden.

## Paso 1. Instala la aplicación

1. Descarga el instalador `Setup.exe` desde la página de descargas.
2. Haz doble clic en el archivo `Setup.exe`.
3. Si aparece una ventana azul de **SmartScreen** («Windows protegió tu PC»), pulsa **Más información** y luego **Ejecutar de todas formas**. Es un aviso habitual para programas nuevos, no un error.
4. Espera a que termine la instalación. No hacen falta permisos de administrador: el instalador comprueba tu sistema y lo prepara todo.

**Qué ocurre después.** Aparece un icono de FarmPanel en el escritorio y en el menú Inicio.

![la ventana del instalador Setup.exe](../images/setup-installer.png)

## Paso 2. Abre la aplicación

Haz doble clic en el icono de **FarmPanel** en el escritorio.

**Qué verás.** En el primer inicio, mientras la licencia aún no está activada, se abre la **ventana de activación** (Activation Wizard). La pantalla principal aparece solo tras una activación correcta.

## Paso 3. Activa tu licencia

La ventana de activación te guía paso a paso.

1. Escribe o pega tu clave de licencia en el campo de entrada. Para pegarla desde el portapapeles, pulsa **Paste from clipboard** (Pegar del portapapeles).
2. La aplicación comprueba el formato de la clave mientras escribes. Cuando el formato es correcto, el botón de activación se habilita.
3. Pulsa **Activate** (Activar).

**Qué ocurre después.** La aplicación contacta con el servidor de licencias y verifica la clave. Esto tarda unos segundos; verás el estado **Activating** (Activando).

**Señal de éxito.** La ventana de activación se cierra y se abre la pantalla principal de la aplicación (**Dashboard**). Tu licencia está activada; no tendrás que volver a introducir la clave en inicios posteriores.

> **Si la activación falla**, la aplicación muestra un mensaje claro y te indica qué hacer. Los casos frecuentes se tratan en [10. Errores y solución de problemas](#10-errores-y-solución-de-problemas).

![la ventana de activación de la licencia](../images/license-activation.png)

## Paso 4. Revisa los ajustes básicos

Antes de iniciar cuentas por primera vez, conviene revisar los ajustes.

1. Pulsa **Settings** (Ajustes) en el panel izquierdo, o pulsa `Ctrl+,`.
2. Abre la sección **Sandboxes** (Sandboxes) y, si hace falta, elige una carpeta para las sandboxes.
3. Si quieres, abre **Appearance** (Apariencia) y elige un tema (**System / Dark / Light**) y la densidad de la interfaz.

Los ajustes se guardan automáticamente: tras cada cambio aparece una breve notificación **Saved** (Guardado).

## Paso 5. Listo para usar

Ya puedes añadir cuentas e iniciar tu primera granja. Consulta [5. Flujos de trabajo principales](#5-flujos-de-trabajo-principales) para saber cómo.

**Señal de que todo funciona.** La barra inferior de la ventana (la barra de estado) muestra un resumen: el número de cuentas, los procesos activos y la versión actual de la aplicación.

---

# 4. Descripción de la interfaz

La aplicación funciona en una única ventana principal. Consta de elementos fijos que están siempre presentes y de un área de pantalla que cambia según la sección que elijas.

```
┌────────────────────────────────────────────────────────────┐
│  Barra de comandos (Command Bar)                            │
├──────────┬─────────────────────────────────────────────────┤
│          │                                                 │
│ Barra    │   Área de trabajo de la pantalla seleccionada   │
│ lateral  │                                                 │
│          │                                                 │
├──────────┴─────────────────────────────────────────────────┤
│  Barra de estado (Status Bar)                               │
└────────────────────────────────────────────────────────────┘
```

![estructura general de la ventana con las áreas etiquetadas](../images/window-layout.png)

## 4.1. Barra de comandos (Command Bar)

**Propósito.** Una franja fija en la parte superior de la ventana. Contiene la navegación, la búsqueda global y las notificaciones.

**Ubicación.** La fila superior de la ventana.

**Elementos principales (de izquierda a derecha):**

- **Botón de menú (☰)** — contrae y expande la barra lateral. Atajo `Ctrl+B`.
- **Logotipo** — al hacer clic vuelves a la pantalla principal (**Dashboard**).
- **Ruta de navegación** — muestra dónde estás, por ejemplo `Accounts › alex_42 › Events`. Haz clic en cualquier segmento para saltar a él.
- **Búsqueda / paleta de comandos** — en el centro. Pulsa `Ctrl+K` para abrir la paleta de comandos (ver más abajo).
- **Indicador de notificaciones** — un icono con un contador (por ejemplo, `⚠ 3`). Al hacer clic se abre el centro de notificaciones.

**Cuándo usarla.** La barra de comandos siempre está a mano: para saltar rápido entre pantallas, buscar una cuenta por su usuario o ejecutar un comando sin ratón.

### Paleta de comandos (Command Palette)

Pulsa `Ctrl+K` en cualquier momento para abrir la paleta de comandos, un cuadro de búsqueda de todas las acciones y objetos de la aplicación.

1. Empieza a escribir el nombre de un comando, una pantalla, el usuario de una cuenta o un flujo de trabajo.
2. La lista se reduce a los resultados que coinciden. Muévete con `↑` `↓`.
3. Pulsa `Enter` para ejecutar el elemento seleccionado.

**Por qué es útil.** La paleta de comandos es la forma más rápida de encontrar cualquier cosa sin memorizar dónde están los botones.

![la paleta de comandos abierta](../images/command-palette.png)

## 4.2. Barra lateral (Sidebar)

**Propósito.** La navegación principal de la aplicación.

**Ubicación.** A la izquierda, a toda la altura de la ventana.

**Secciones (de arriba abajo):**

| Icono | Sección | Qué muestra |
|---|---|---|
| ▤ | **Dashboard** | Resumen de toda la granja |
| 👥 | **Accounts** | Lista de todas las cuentas (la pantalla de trabajo principal) |
| ⚙ | **Workflows** | Escenarios de inicio automatizados y su progreso |
| ⚔ | **Matchmaking** | Grupos (party) y búsqueda de partida |
| 📈 | **Monitoring** | Carga del equipo y estado de los procesos |
| 📜 | **Logs** | El registro de eventos |
| ▣ | **Layouts** | Distribución de las ventanas de CS2 por los monitores |
| ▦ | **Sandboxes** | Sandboxes (entornos aislados) |
| ⚙ | **Settings** | Ajustes de la aplicación |
| ? | **Help** | Ayuda |

Junto a algunas secciones se muestra un contador (por ejemplo, el número de cuentas) o un punto activo cuando hay actividad.

**Acciones principales:**

- Haz clic en una sección para abrirla. También puedes usar `Ctrl+1`…`Ctrl+8`.
- El botón de contraer (o `Ctrl+B`) reduce el panel a iconos para ganar espacio.

**Consejo.** Cambiar de sección conserva tu estado: filtros, selección y posición de desplazamiento. Al volver a una pantalla, la encuentras tal como la dejaste.

![la barra lateral con todas las secciones](../images/sidebar.png)

## 4.3. Barra de estado (Status Bar)

**Propósito.** Una franja fina en la parte inferior de la ventana con un resumen rápido del estado de toda la granja.

**Ubicación.** La fila inferior de la ventana.

**Qué muestra (ejemplo):**

```
[env: PROD] | ● 412 cuentas (238 en marcha) | ▶ 18 workflows | ◎ 7 partidas | CPU 42% RAM 71% | ⚠ 3 errores | 14:32:08 | v1.0.1
```

- cuántas cuentas existen y cuántas están en marcha ahora;
- cuántos workflows y partidas activas hay en curso;
- carga del procesador y de la memoria;
- el número de errores (haz clic para abrir el centro de notificaciones);
- la hora y la versión de la aplicación.

**Cuándo usarla.** Echa un vistazo a la barra de estado para saber en un segundo si todo va bien.

## 4.4. Pantalla Dashboard (Resumen principal)

**Propósito.** Una única pantalla de resumen. En pocos segundos responde: cuántas cuentas están en línea, cuántos workflows están en marcha o han fallado, si hay actividad de emparejamiento, si hay caídas y cuánta carga tiene el equipo.

**Ubicación.** La primera sección de la barra lateral. Se abre justo después del inicio.

**Áreas principales:**

- **Franja de indicadores (KPI)** — cinco tarjetas en la parte superior: **Accounts**, **Workflows**, **Matches**, **Errors**, **System**. Cada una muestra una cifra principal y un minigráfico. Al hacer clic en una tarjeta vas a la pantalla correspondiente.
- **Live Activity Feed** (Actividad en vivo) — un flujo de eventos operativos en tiempo real. Con el botón de pausa (o la tecla `Space`) puedes detener el desplazamiento.
- **Account State Heatmap** (Mapa de estados) — una cuadrícula donde cada cuenta es una celda de color. El color refleja su estado. Pasa el cursor para ver el usuario y el estado; haz clic para saltar a la cuenta.
- **Active Workflows / Matchmaking Queue / Sandboxes** — tres paneles que resumen los workflows, la cola de partidas y las sandboxes.
- **Failures & Crashes** (Fallos y caídas) — una tabla de errores y caídas recientes de la última hora.

**Uso típico.** Por la mañana, abre el **Dashboard** para evaluar la granja de un vistazo y luego ve donde se necesite atención.

**Consejos.**
- Los indicadores se actualizan automáticamente. Para forzar una actualización completa, pulsa `F5`.
- Si algo aparece resaltado en rojo en la tarjeta **Errors** o en la tabla de fallos, empieza el análisis por ahí.

![el Dashboard con la franja de indicadores y la actividad en vivo](../images/dashboard-screen.png)

## 4.5. Pantalla Accounts (Cuentas)

**Propósito.** La pantalla de trabajo principal. Aquí guardas las cuentas, encuentras las que necesitas y las inicias y detienes.

**Ubicación.** La segunda sección de la barra lateral (`Ctrl+2`).

**Áreas principales:**

- **Barra de herramientas (Toolbar)** — los botones **Add Account**, **Import**, **Export** y **Refresh**, el campo de búsqueda, los filtros y los controles de vista.
- **Tabla de cuentas** — una lista de todas las cuentas con columnas: estado, usuario, apodo, rango, workflow, sandbox, etiquetas, hora del último inicio de sesión y otras.
- **Details Pane** (Panel de detalles) — a la derecha. Muestra los detalles de la cuenta seleccionada. Muéstralo u ocúltalo con `Ctrl+\`.

**Qué puedes hacer:**

- Añadir cuentas de una en una o importar una lista.
- Buscar y filtrar cuentas.
- Iniciar, detener y reiniciar una cuenta o muchas a la vez.
- Vincular cuentas a sandboxes y asignar workflows.
- Ver una ficha detallada de la cuenta: datos, historial, eventos y registro.

**Uso típico.** Selecciona las cuentas que necesites en la tabla y luego ejecuta una acción sobre ellas mediante la barra de herramientas, el menú contextual (clic derecho) o los atajos de teclado.

Las instrucciones detalladas paso a paso están en [5. Flujos de trabajo principales](#5-flujos-de-trabajo-principales).

![la pantalla Accounts con la tabla y el panel de detalles](../images/accounts-screen.png)

### Panel de detalles de la cuenta (Details Pane)

A la derecha de la tabla aparece una ficha de la cuenta seleccionada con estas pestañas:

| Pestaña | Qué muestra |
|---|---|
| **Overview** | Datos principales, vínculo de sandbox, workflow asignado, etiquetas, fechas clave y botones de acción |
| **Inventory** | El inventario de la cuenta: número de objetos y su valor |
| **Workflow** | El estado actual del escenario asignado y su paso actual |
| **Events** | Eventos recientes de esta cuenta |
| **Logs** | El registro de eventos filtrado por esta cuenta |
| **History** | Historial de cambios: creación, ediciones, cambios de nombre, revínculos de sandbox |

En la parte inferior de la pestaña **Overview** hay un bloque de botones: **Start**, **Stop**, **Restart**, **Pause**, además de **Edit account** y **Delete**. La acción más relevante aparece resaltada: **Start** cuando la cuenta está detenida y **Stop** cuando está en marcha.

## 4.6. Pantalla Workflows (Escenarios)

**Propósito.** Gestionar los escenarios de inicio automatizados y observar su ejecución.

**Ubicación.** La tercera sección de la barra lateral (`Ctrl+3`).

**Qué es un workflow.** Un workflow (escenario) es una secuencia de pasos predefinida que la aplicación ejecuta para una cuenta: iniciar sesión en Steam, lanzar CS2, etc. El mismo escenario se ejecuta siempre igual, por lo que el resultado es predecible.

- **Definition** (Definición) — la plantilla del escenario: un conjunto de pasos.
- **Instance** (Instancia) — una única ejecución de una definición para una cuenta concreta.

**Áreas principales:**

- **A la izquierda** — una lista de definiciones (plantillas) y sus versiones.
- **En el centro** — una tabla de instancias en ejecución: qué escenario, para qué cuenta, en qué paso, cuántos reintentos, cuándo se inició.
- **A la derecha** — los detalles de la instancia seleccionada (pestañas **Overview**, **State Machine**, **Steps**, **Logs**, **Retries**).
- **Abajo** — una línea de tiempo de eventos plegable para las instancias visibles (`Ctrl+T`).

**Cuándo usarla.** Ven aquí para ver en qué paso está el inicio de cada cuenta, pausar o reiniciar un escenario, o averiguar por qué algo no terminó.

![la pantalla Workflows con tres paneles](../images/workflows-screen.png)

## 4.7. Pantalla Matchmaking (Búsqueda de partida)

**Propósito.** Formar grupos de cuentas (party) y ponerlos en cola de emparejamiento juntos.

**Ubicación.** La cuarta sección de la barra lateral (`Ctrl+4`).

**Conceptos clave:**

| Término | Significado |
|---|---|
| **Party** (Grupo) | Un conjunto de cuentas que buscan partida juntas |
| **Quorum** (Cuórum) | Todos los miembros del grupo han iniciado sesión, están en cola y no están en partida |
| **Queue** (Cola) | La espera de partida: posición, región, modo |
| **Match Found** (Partida encontrada) | Steam encontró una partida. La aplicación confirma la disposición de todos los miembros automáticamente; no tienes que hacer nada |
| **Desync** (Desincronización) | Los miembros están en un estado inconsistente (por ejemplo, alguien salió de la cola) |

**Áreas principales:**

- **A la izquierda** — una lista de grupos con su estado (cuórum, desincronización, partida encontrada, inactivo).
- **A la derecha** — los detalles del grupo seleccionado: miembros, su estado, posición en la cola, latencia de red, sandbox.
- **Abajo** — una línea de tiempo de eventos recientes de emparejamiento.

**Cuándo usarla.** Aquí formas grupos de 2–5 cuentas y los pones en cola. Cuando se encuentra una partida, la aplicación confirma la disposición de todos los miembros automáticamente.

![la pantalla Matchmaking con grupos y detalles](../images/matchmaking-screen.png)

## 4.8. Pantalla Monitoring (Supervisión)

**Propósito.** Vigilar la carga del equipo, el estado de los procesos y las caídas en tiempo real.

**Ubicación.** La quinta sección de la barra lateral (`Ctrl+5`).

**Áreas principales:**

- **Medidores de recursos** — tarjetas de **CPU**, **RAM**, **Disk**, **Net** y, si está disponible, **GPU**, con los valores actuales y minigráficos.
- **Process Explorer** (Explorador de procesos) — una tabla de todos los procesos de Steam y CS2 en ejecución: a qué cuenta pertenece cada uno, cuánto consume y cuánto lleva funcionando.
- **Crashes & Warnings** (Caídas y avisos) — un flujo de fallos recientes.
- **Logs panel** (Panel de registro) — un registro en la parte inferior de la pantalla, que se puede plegar.

**Controles de tiempo.** Arriba puedes cambiar entre **Live** (tiempo real), **Last 1h / 24h** (última hora/día) y **Custom** (un periodo personalizado). El botón **Freeze** (`Ctrl+Space`) congela la imagen para estudiarla con calma.

**Cuándo usarla.** Si el equipo empieza a ir lento o las caídas se vuelven frecuentes, abre **Monitoring** para ver qué proceso consume recursos y qué se ha caído exactamente.

> **Consejo.** Puedes abrir la pantalla **Monitoring** en una ventana aparte con el botón de desacoplar y colocarla en un segundo monitor.

![la pantalla Monitoring con medidores y la lista de procesos](../images/monitoring-screen.png)

## 4.9. Pantalla Logs (Registro)

**Propósito.** Un registro detallado de todos los eventos de la aplicación, como un flujo en vivo de lo que ocurre.

**Ubicación.** La sexta sección de la barra lateral (`Ctrl+6`).

**Funciones principales:**

- **Filtro por nivel** — los interruptores **Error**, **Warn**, **Info**, **Debug**. Por defecto se muestran errores, avisos y mensajes informativos.
- **Filtro por origen** — puedes limitar el registro a una sola cuenta, workflow o sandbox.
- **Búsqueda** — `Ctrl+F`, con salto entre coincidencias (`F3` / `Shift+F3`).
- **Follow** (Seguir) — el registro se desplaza automáticamente hacia las líneas nuevas. La tecla `Space` activa y desactiva el seguimiento. Si te desplazas hacia arriba, el seguimiento se pausa y aparece un botón para volver abajo.
- **Export** (Exportar) — guarda las líneas visibles en un archivo.

**Cuándo usarla.** Cuando necesitas los detalles: qué le pasó exactamente a una cuenta concreta y en qué orden.

![la pantalla Logs con un registro de eventos](../images/logs-screen.png)

## 4.10. Pantalla Layouts (Distribución de ventanas)

**Propósito.** Distribuir las ventanas de CS2 por uno o varios monitores según un diseño predefinido.

**Ubicación.** La séptima sección de la barra lateral (`Ctrl+7`).

**Conceptos clave:**

- **Preset** (Preajuste) — una distribución de ventanas guardada.
- **Slot** (Hueco) — un área rectangular de un monitor donde irá una ventana.
- **Snap** (Ajustar) — el comando que coloca las ventanas en ejecución en los huecos.

**Áreas principales:**

- **A la izquierda** — una lista de preajustes guardados.
- **A la derecha** — un lienzo que muestra tus monitores, en el que colocas los huecos.
- **Abajo** — una tabla de asignaciones: qué hueco corresponde a qué cuenta o rol.

**Cómo usarla.**
1. Crea un preajuste con el botón **New Preset**.
2. Coloca los huecos en el lienzo.
3. Define qué cuenta va en cada hueco.
4. Pulsa **Apply** (Aplicar) o **Snap windows** (Ajustar ventanas): la aplicación coloca las ventanas de CS2 en ejecución en los lugares definidos.

> **Red de seguridad.** Antes de distribuir, la aplicación recuerda las posiciones actuales de las ventanas. El botón **Revert layout** (Revertir distribución) restaura las posiciones anteriores durante un minuto.

![la pantalla Layouts con el lienzo de monitores](../images/layouts-screen.png)

## 4.11. Pantalla Sandboxes (Sandboxes)

**Propósito.** Gestionar las sandboxes: los entornos aislados en los que se ejecutan los clientes de Steam.

**Ubicación.** La octava sección de la barra lateral (`Ctrl+8`).

**Qué es una sandbox.** Una sandbox es un entorno separado y protegido para un cliente de Steam. Las cuentas en sandboxes distintas nunca se solapan: no comparten sesiones, archivos ni rastros. Una cuenta se vincula a una sandbox.

**Cuándo usarla.** Aquí creas sandboxes y vigilas su estado. En la mayoría de los casos las sandboxes se asignan automáticamente al añadir cuentas, así que rara vez necesitas venir aquí a propósito.

## 4.12. Pantalla Settings (Ajustes)

**Propósito.** Adaptar la aplicación a tus preferencias.

**Ubicación.** La sección **Settings** en la parte inferior de la barra lateral (`Ctrl+,`).

**Distribución.** A la izquierda hay una lista de secciones de ajustes; a la derecha, los ajustes en sí. Los cambios se guardan de inmediato: tras cada uno aparece una breve notificación **Saved**.

**Secciones de ajustes:**

| Sección | Qué configura |
|---|---|
| **General** | Inicio junto con Windows, minimizar a la bandeja, canal de actualizaciones |
| **Appearance** | Tema (**System / Dark / Light**), densidad, escala de fuente, reducción de animaciones |
| **Accounts** | Comportamiento al crear cuentas, retención de las eliminadas |
| **Workflows** | Política de reintentos, límites de ejecuciones simultáneas |
| **Sandboxes** | Carpeta de sandboxes, recuperación automática |
| **Monitoring** | Frecuencia de actualización de datos, umbrales de aviso |
| **Notifications** | Notificaciones y sonidos por nivel de gravedad |
| **Layouts** | Distribuciones por defecto, comportamiento con varios monitores |
| **Hotkeys** | Atajos de teclado; se pueden reasignar |
| **Advanced** | Nivel de registro, diagnóstico, selección de entorno, restablecer valores por defecto |
| **About** | Versión de la aplicación, botones para abrir las carpetas de datos y de registros |

> **Nota.** Algunos ajustes (por ejemplo, la carpeta de sandboxes o el entorno) solo se aplican tras reiniciar. Esos ajustes muestran una etiqueta «Requires restart» (Requiere reinicio).

![la pantalla Settings](../images/settings-screen.png)

---

# 5. Flujos de trabajo principales

Esta es la sección más importante. Contiene instrucciones completas paso a paso para las tareas principales. Cada paso describe qué verás y cómo confirmar el éxito.

## 5.1. Añadir una sola cuenta

**Objetivo.** Añadir una cuenta de Steam nueva a la aplicación.

**Qué necesitas.** El usuario y la contraseña de la cuenta. Un código de Steam Guard si corresponde.

### Paso 1 — Abre el formulario de alta

Ve a la pantalla **Accounts** y pulsa **Add Account** (Añadir cuenta) en la barra de herramientas. También puedes pulsar `Ctrl+N`.

**Resultado esperado.** Se abre un formulario con campos para la nueva cuenta.

### Paso 2 — Rellena los datos

Rellena los campos:

- **Login** (Usuario) — obligatorio, debe ser único.
- **Password** (Contraseña) — obligatorio.
- **Steam Guard secret** — el código de Steam Guard, si lo tienes (opcional).
- **Nickname** (Apodo) — opcional; puede obtenerse automáticamente en el primer inicio de sesión.
- **Tags** (Etiquetas) — etiquetas opcionales para agrupar.
- **Sandbox binding** (Sandbox) — elige **Auto-assign** (Asignar automáticamente), una sandbox concreta o **None** (Ninguna).
- **Workflow** — el escenario de inicio, si quieres asignarlo de inmediato.

**Resultado esperado.** Si el usuario ya está en uso, el campo se resalta en rojo con una explicación. Una contraseña débil se resalta en ámbar; es un aviso y no impide guardar.

### Paso 3 — Guarda la cuenta

Pulsa el botón de guardar del formulario.

**Resultado esperado.** El formulario se cierra y la nueva cuenta aparece en la tabla con el estado **Draft** (Borrador) o, si está vinculada a una sandbox, lista para iniciar.

**Señal de éxito.** La cuenta es visible en la tabla de la pantalla **Accounts**.

### Consejos

- Si activas **Validate immediately** (Validar de inmediato) en el formulario, la aplicación comprueba el inicio de sesión en segundo plano y muestra el resultado como notificación.
- Para que una cuenta se pueda iniciar, debe estar vinculada a una sandbox. La opción más sencilla es **Auto-assign**.

### Errores frecuentes y cómo resolverlos

- **«El usuario ya está en uso».** Ese usuario ya existe en la aplicación. Revisa tu lista de cuentas; puede que ya lo hayas añadido.
- **Olvidaste la sandbox.** Una cuenta sin sandbox no se puede iniciar. Vincula una más tarde desde el menú contextual → **Bind sandbox**.

![el formulario de alta de cuenta](../images/accounts-add-form.png)

## 5.2. Importar una lista de cuentas desde un archivo

**Objetivo.** Añadir rápidamente muchas cuentas a la vez desde un archivo.

**Qué necesitas.** Un archivo con una lista de cuentas (TXT, CSV o TSV). El formato de línea TXT más sencillo es `usuario:contraseña` (también puedes usar `usuario:contraseña:steamguard:apodo`).

### Paso 1 — Inicia el asistente de importación

En la pantalla **Accounts**, pulsa la flecha junto al botón **Import** (Importar) y elige un origen; por ejemplo, **From file…** (Desde archivo). También puedes pulsar `Ctrl+I`.

**Resultado esperado.** Se abre un asistente de importación paso a paso.

### Paso 2 — Elige el origen y cómo se asignan las sandboxes

Indica el archivo con el botón **Browse…** (Examinar). En la parte inferior, elige cómo asignar las sandboxes:

- **Auto-assign (round-robin)** — distribuir en ciclo (recomendado);
- **Bind to specific sandbox** — vincularlas todas a una sandbox;
- **Leave unbound** — dejarlas sin sandbox.

Pulsa Siguiente.

### Paso 3 — Comprueba cómo se reconocieron los datos

El asistente muestra las primeras filas del archivo como una tabla. Asegúrate de que los datos se dividieron en columnas correctamente. Si el delimitador se detectó mal, defínelo a mano.

**Resultado esperado.** En la vista previa, los usuarios y las contraseñas están en sus propias columnas.

### Paso 4 — Asigna los campos

Arrastra los encabezados de columna a las casillas requeridas: **Login**, **Password**, **SteamGuard**, **Nickname**.

### Paso 5 — Comprueba que las filas son válidas

El asistente marca cada fila: ✓ válida, ⚠ aviso, ✕ error. Las filas con errores se pueden corregir aquí mismo u omitir.

**Resultado esperado.** Ves cuántas cuentas se añadirán, cuántas son duplicadas y cuántas tienen errores.

### Paso 6 — Confirma la importación

Pulsa **Import N accounts** (Importar N cuentas).

**Resultado esperado.** Aparece una barra de progreso con el estado de cada fila. Al terminar, las cuentas aparecen en la tabla.

**Señal de éxito.** El número de cuentas de la tabla ha aumentado en la cantidad importada.

### Cómo cancelar y recuperar

Si cancelas la importación mientras se ejecuta, la aplicación ofrece revertir el lote ya añadido. Confirma la reversión para volver al estado original.

![el asistente de importación, paso de validación de filas](../images/import-wizard-validation.png)

## 5.3. Iniciar varias cuentas

**Objetivo.** Iniciar varias cuentas al mismo tiempo.

**Qué necesitas.** Cuentas ya añadidas y vinculadas a sandboxes.

### Paso 1 — Selecciona las cuentas

En la pantalla **Accounts**, marca las cuentas que quieras en la primera columna. Para seleccionar todas las visibles, pulsa `Ctrl+A`.

**Resultado esperado.** La barra de herramientas cambia al modo de operaciones masivas y muestra cuántas filas están seleccionadas, por ejemplo `12 selected`.

### Paso 2 — Inicia las cuentas seleccionadas

Pulsa **Start** (Iniciar) en la barra de operaciones masivas. También puedes pulsar `Ctrl+R`.

**Resultado esperado.** El estado de las cuentas seleccionadas cambia a **Starting** (Iniciando). La aplicación prepara cada cuenta y comienza el inicio. El inicio se hace por lotes para no sobrecargar el equipo.

### Paso 3 — Espera al inicio

Observa la columna de estado. Espera a que las cuentas pasen al estado **Running** (En marcha).

**Resultado esperado.** Las cuentas iniciadas muestran **Running**, con un contador de tiempo de actividad al lado.

**Señal de éxito.** Todas las cuentas seleccionadas muestran **Running**. El número de activas en la barra de estado ha aumentado.

### Consejos

- No tienes que iniciar todas las cuentas a la vez. Empieza con un lote pequeño, comprueba que todo es estable y luego añade más.
- Para iniciar una sola cuenta: selecciona una fila y pulsa **Start**, o usa el botón **Start** del panel de detalles a la derecha.

### Errores frecuentes y recuperación

- **Una cuenta se queda en Starting demasiado tiempo.** El inicio de sesión puede ir lento. Espera; si el estado cambia a **Error**, usa el botón **Retry** (Reintentar).
- **Algunas cuentas no se iniciaron.** Tras un inicio masivo, un resumen muestra cuántas tuvieron éxito y cuántas fallaron. Pulsa **Filter to failed** (Mostrar solo las fallidas) para ocuparte solo de esas.

![inicio masivo de cuentas, estados Starting/Running](../images/accounts-bulk-start.png)

## 5.4. Detener todas las cuentas en marcha

**Objetivo.** Cerrar de forma ordenada todas las cuentas activas.

### Paso 1 — Selecciona las cuentas

Selecciona las cuentas en marcha. Para seleccionar todas las visibles, pulsa `Ctrl+A`.

### Paso 2 — Detenlas

Pulsa **Stop** (Detener) en la barra de operaciones masivas, o pulsa `Ctrl+.` (Ctrl y punto).

**Resultado esperado.** La aplicación cierra de forma ordenada cada cuenta. El estado cambia a **Stopped** (Detenida). Si una cuenta no responde, al cabo de un rato la aplicación la cierra por la fuerza.

**Señal de éxito.** Todas las cuentas muestran **Stopped**. El número de activas en la barra de estado ha disminuido.

### Consejos

- **Stop** es un cierre ordenado. La aplicación primero intenta cerrar los clientes correctamente.
- Si una cuenta está en partida, termina primero las acciones dentro del juego y luego detenla.

## 5.5. Crear un grupo (party) y ponerlo en cola

**Objetivo.** Formar un grupo de varias cuentas y ponerlas en cola de emparejamiento juntas.

**Qué necesitas.** Varias cuentas en marcha (**Running**) que hayan iniciado sesión.

### Paso 1 — Crea un grupo

Ve a la pantalla **Matchmaking** y pulsa **Create Party** (Crear grupo). También puedes pulsar `Ctrl+N`.

**Resultado esperado.** Se abre una ventana donde puedes añadir cuentas al grupo y darle un nombre.

### Paso 2 — Añade miembros y guarda

Añade de 2 a 5 cuentas al grupo, ponle un nombre y guarda.

**Resultado esperado.** El nuevo grupo aparece en la lista de la izquierda.

### Paso 3 — Comprueba el cuórum

Selecciona el grupo y mira sus miembros a la derecha. Asegúrate de que el grupo está en el estado **Quorum** (Cuórum), es decir, todos los miembros han iniciado sesión y están listos.

**Resultado esperado.** El grupo muestra una insignia **✓ Quorum**. Si un miembro tiene un problema (por ejemplo, un inicio de sesión lento), se muestra en una línea aparte.

### Paso 4 — Pon el grupo en cola

Pulsa **Queue** para el grupo seleccionado (o `Ctrl+Q`). Para poner en cola todos los grupos a la vez, usa **Queue All** en la barra de herramientas.

**Resultado esperado.** Antes de la cola, la aplicación realiza sus comprobaciones. Después todos los miembros entran en la cola, con sus posiciones y la latencia de red visibles.

**Señal de éxito.** Los miembros están en estado de cola, con un contador de tiempo de espera en marcha.

### Consejos

- Elige la región y el modo en la barra de herramientas (por ejemplo, `EU` y `Premier`) antes de la cola.
- Si el grupo entra en el estado **Desync** (Desincronización), usa la acción **Re-sync** (Resincronizar) para pausar la cola y esperar un estado consistente.

![un grupo en la cola con las posiciones de los miembros](../images/matchmaking-party-queue.png)

## 5.6. Qué ocurre cuando se encuentra una partida

**Objetivo.** Entender qué hace la aplicación en el momento en que se encuentra una partida.

**Qué necesitas.** Un grupo que esté en la cola.

### La aceptación de la partida es automática

Cuando Steam encuentra una partida, aparece una banda destacada **MATCH FOUND** (Partida encontrada) para el grupo. **No tienes que pulsar nada**: la aplicación confirma la disposición de todos los miembros del grupo dentro del plazo. No se requiere ninguna acción por tu parte.

**Resultado esperado.** Los miembros del grupo aceptan la partida automáticamente; su estado cambia a **✓ Accepted** (Aceptado).

**Señal de éxito.** Todos los miembros muestran **Accepted** y la partida comienza.

> **Consejo.** ¿Quieres enterarte de que se encontró una partida sin mirar la pantalla? Activa una alerta de sonido para **Match found** en **Settings → Notifications**. La aceptación se produce igualmente de forma automática; el sonido solo sirve para mantenerte informado.

### Qué hacer si el grupo se desincroniza

A veces no se puede confirmar la partida para todos; por ejemplo, si un miembro salió de la cola. Entonces el grupo entra en el estado **Desync** (Desincronización). Usa la acción **Re-sync** (Resincronizar) y, si hace falta, quita al miembro problemático con **Drop member** (Quitar miembro) y vuelve a poner al resto en cola.

![la banda Match Found](../images/matchmaking-match-found.png)

## 5.7. Recuperarse tras una caída o reinicio de la aplicación

**Objetivo.** Devolver la granja a un estado operativo tras la caída de un cliente, o tras cerrar y volver a abrir la aplicación.

**Qué necesitas.** Nada más: la recuperación ocurre en gran medida de forma automática.

### Qué ocurre automáticamente

- **Tras la caída de un cliente.** Si Steam o CS2 se cierran de forma inesperada, la aplicación lo detecta, marca la cuenta con el estado **Crashed** (Caída) y muestra una notificación con un botón **Restart** (Reiniciar). La recuperación suele producirse sola en unos segundos.
- **Tras reiniciar la aplicación.** Al arrancar, la aplicación busca procesos de Steam y CS2 que quedaron de la sesión anterior y vuelve a tomarlos bajo su gestión. Mientras tanto, aparece un indicador **Recovering** (Recuperando) en la barra de estado. Las cuentas readmitidas se marcan como «Reattached» durante un breve tiempo.

### Qué hacer manualmente

1. Abre el **Dashboard** y mira la tabla **Failures & Crashes**.
2. Para una cuenta caída, pulsa **Restart** en la notificación, en la fila de la cuenta o en el panel de detalles.
3. Si la aplicación informa de un proceso huérfano (**Orphan process**) en el centro de notificaciones, elige **Adopt** (Adoptar) o **Kill** (Terminar).

**Señal de éxito.** Las cuentas vuelven a estar en estado **Running**, las marcas rojas de caída han desaparecido y no hay un indicador **Recovering** activo en la barra de estado.

### Consejos

- No relances todo a mano justo después de una caída: primero dale a la recuperación automática unos segundos.
- Si las caídas se repiten, abre **Monitoring** para ver la carga: puede que estés ejecutando más cuentas de las que este equipo puede soportar.

![el indicador Recovering en la barra de estado](../images/status-recovering.png)

---

# 6. Tareas habituales («Quiero…»)

Respuestas breves a objetivos comunes. Para instrucciones completas, sigue los enlaces a la sección 5.

## «Quiero añadir cuentas nuevas»

- **Cuándo lo necesitas.** Tienes cuentas de Steam nuevas.
- **Qué hacer.** Para una cuenta, usa el botón **Add Account** en la pantalla **Accounts**. Para muchas a la vez, usa el botón **Import** y el asistente de importación.
- **Qué ocurre.** Las cuentas aparecen en la tabla y quedan listas para iniciar (una vez que tienen sandbox).
- Más: [5.1](#51-añadir-una-sola-cuenta), [5.2](#52-importar-una-lista-de-cuentas-desde-un-archivo).

## «Quiero iniciar Steam»

- **Cuándo lo necesitas.** Necesitas que una cuenta inicie sesión en Steam.
- **Qué hacer.** Selecciona la cuenta en la pantalla **Accounts** y pulsa **Start**.
- **Qué ocurre.** La aplicación inicia Steam en la sandbox de la cuenta e inicia sesión. El estado pasa de **Starting → Running**.

## «Quiero iniciar CS2»

- **Cuándo lo necesitas.** Steam ya está en marcha y necesitas iniciar el juego.
- **Qué hacer.** Iniciar la cuenta con **Start** la lleva por todo el escenario, incluido el inicio de CS2 (si el workflow asignado lo contempla).
- **Qué ocurre.** Tras iniciar sesión en Steam, la aplicación inicia CS2. Puedes seguir los pasos en la pantalla **Workflows**.

## «Quiero crear una sala»

- **Cuándo lo necesitas.** Necesitas reunir cuentas en una sala de juego.
- **Qué hacer.** Forma un grupo en la pantalla **Matchmaking** con **Create Party** y añade miembros.
- **Qué ocurre.** La aplicación combina las cuentas seleccionadas en un grupo y ayuda a llevarlas a un estado consistente (cuórum).
- Más: [5.5](#55-crear-un-grupo-party-y-ponerlo-en-cola).

## «Quiero empezar la búsqueda de partida»

- **Cuándo lo necesitas.** El grupo está formado y listo.
- **Qué hacer.** Selecciona el grupo y pulsa **Queue** (o **Queue All** para todos).
- **Qué ocurre.** Los miembros entran en la cola; ves sus posiciones y el tiempo de espera.

## «Quiero detener todas las sesiones en marcha»

- **Cuándo lo necesitas.** Es hora de terminar.
- **Qué hacer.** Selecciona las cuentas (`Ctrl+A`) y pulsa **Stop**.
- **Qué ocurre.** La aplicación cierra los clientes de forma ordenada y los estados pasan a **Stopped**.
- Más: [5.4](#54-detener-todas-las-cuentas-en-marcha).

## «Quiero recuperarme tras una caída»

- **Cuándo lo necesitas.** Un cliente se cayó o la aplicación se reinició.
- **Qué hacer.** Dale a la recuperación automática unos segundos; si hace falta, pulsa **Restart** para la cuenta caída.
- **Qué ocurre.** La aplicación devuelve las cuentas al trabajo.
- Más: [5.7](#57-recuperarse-tras-una-caída-o-reinicio-de-la-aplicación).

## «Quiero distribuir las ventanas en pantalla»

- **Cuándo lo necesitas.** Quieres colocar de forma ordenada las ventanas de CS2 en tu monitor.
- **Qué hacer.** En la pantalla **Layouts**, crea un preajuste y pulsa **Apply** / **Snap windows**.
- **Qué ocurre.** Las ventanas en marcha se colocan en los lugares definidos.

---

# 7. Referencia de funciones

Esta sección cubre funciones concretas con su propósito, ubicación y particularidades.

## 7.1. Búsqueda y filtros de cuentas

**Propósito.** Encontrar rápidamente las cuentas que necesitas en una lista grande.

**Ubicación.** La barra de herramientas de la pantalla **Accounts**: el campo de búsqueda y el botón **Filters**.

**Cómo usarlo.**
- Escribe en el campo de búsqueda (`Ctrl+F`). Puedes buscar por partes: `login:alex`, `status:running`, `rank:>=gold`, `tag:prime`.
- Pulsa **Filters** (`Ctrl+K` en esta pantalla abre la ventana de filtros), define condiciones por estado, rango, sandbox, workflow o etiquetas, y guarda el conjunto como un preajuste.

**Comportamiento esperado.** La tabla muestra de inmediato solo las cuentas que coinciden. Los filtros activos aparecen como una fila de fichas debajo de la barra de herramientas.

**Consejo.** Guarda los conjuntos de condiciones que uses a menudo como preajustes; están disponibles en el desplegable de la barra de herramientas.

## 7.2. Agrupación y configuración de columnas

**Propósito.** Organizar la tabla según tu tarea.

**Ubicación.** La barra de herramientas de la pantalla **Accounts**: los botones **Density** (Densidad), **Columns** (Columnas) y **Group** (Agrupar).

**Cómo usarlo.**
- **Group** permite agrupar las cuentas por estado, workflow, sandbox, etiqueta o rango. Los grupos muestran contadores, por ejemplo `Running (24)`.
- **Columns** — el conjunto de columnas visibles. Hay conjuntos predefinidos: **Operational**, **Identity**, **Audit**, **Compact**. Puedes guardar el tuyo.
- **Density** — la altura de las filas (más compacta o más amplia).

## 7.3. Menú contextual de la cuenta

**Propósito.** Acceso rápido a todas las acciones de una cuenta.

**Ubicación.** Haz clic derecho en la fila de una cuenta.

**Qué hay disponible.** Editar, copiar el usuario o el Steam ID, iniciar/detener/reiniciar, vincular y desvincular una sandbox, asignar un workflow, reautenticar (**Re-auth**), probar el inicio de sesión (**Probe login now**), trabajar con etiquetas, exportar, clonar y eliminar.

## 7.4. Operaciones masivas

**Propósito.** Ejecutar una acción sobre muchas cuentas a la vez.

**Ubicación.** La barra de herramientas de la pantalla **Accounts** en modo de selección (cuando al menos una fila está marcada).

**Cómo usarlo.** Marca las cuentas y luego pulsa el botón que necesites: **Start**, **Stop**, **Restart**, **Bind sandbox**, **Workflow…**, **Tag…**, **Export** o **Delete**.

**Comportamiento esperado.** Aparece una ventana con el progreso de cada cuenta. Puedes cancelar la operación mientras se ejecuta.

**Limitación.** Al eliminar cinco cuentas o más, la aplicación pide confirmar escribiendo la palabra `DELETE`.

## 7.5. Exportar cuentas

**Propósito.** Guardar los datos de las cuentas en un archivo.

**Ubicación.** El botón **Export** de la barra de herramientas o del menú contextual.

**Cómo usarlo.** Elige un formato: **TXT** (usuario:contraseña), **CSV** (todos los campos) o **JSON** (el registro completo).

> **Advertencia.** Exportar contraseñas requiere un consentimiento aparte: la aplicación pide marcar una casilla. Maneja esos archivos con cuidado.

## 7.6. Clonar una cuenta

**Propósito.** Crear rápidamente una copia de una cuenta como punto de partida.

**Ubicación.** Menú contextual de la fila → **Clone…**.

**Comportamiento esperado.** Se abre un formulario con los campos ya rellenados (el usuario pasa a ser `original_copy`), salvo el código de Steam Guard y el vínculo de sandbox, que defines de nuevo.

## 7.7. Workflows: iniciar, pausar, detener

**Propósito.** Gestionar los escenarios automatizados.

**Ubicación.** La pantalla **Workflows**.

**Cómo usarlo.**

| Acción | Qué hace | ¿Pide confirmación? |
|---|---|---|
| **Start** | Ejecuta el escenario para las cuentas seleccionadas | Al iniciar más de 10 cuentas |
| **Pause** | Pausa con suavidad tras el paso actual | No |
| **Resume** | Continúa desde el punto actual | No |
| **Stop** | Termina el escenario con limpieza | Sí |
| **Restart** | Detiene y vuelve a empezar | Sí (en operación masiva) |
| **Skip step** | Marca el paso actual como hecho y avanza | Sí |
| **Retry now** | Reintenta el paso actual de inmediato | No |

**Consejo.** La pestaña **State Machine** del panel de detalles muestra con claridad en qué paso está un escenario.

## 7.8. Vincular a una sandbox

**Propósito.** Reservar un entorno aislado para una cuenta, sin el cual no se puede iniciar.

**Ubicación.** Menú contextual → **Bind sandbox…**, o la operación masiva **Bind sandbox**.

**Cómo usarlo.** Elige un método: en ciclo (round-robin), llenar primero las vacías o una sandbox concreta.

**Limitación.** Una cuenta, una sandbox. Si la sandbox elegida ya está en uso, la aplicación ofrece liberarla de la cuenta anterior.

## 7.9. Distribución de ventanas (Layouts)

**Propósito.** Distribuir las ventanas de CS2 según un diseño predefinido.

**Ubicación.** La pantalla **Layouts**.

**Cómo usarlo.** Crea un preajuste, coloca los huecos en el lienzo de monitores, define las asignaciones y pulsa **Apply**.

**Consejo.** El botón **Revert layout** restaura las posiciones anteriores de las ventanas durante un minuto, por si una distribución no salió bien.

## 7.10. Centro de notificaciones

**Propósito.** Un único lugar para todas las notificaciones de la aplicación.

**Ubicación.** El indicador de notificaciones de la barra superior, o `Ctrl+Shift+N`.

**Cómo usarlo.** El panel se abre a la derecha. Cambia entre las pestañas **All**, **Errors**, **Warnings** e **Info**. En cada entrada puedes ir al origen, reintentar o descartar. El botón **Clear all** vacía la lista.

**Limitación.** Se conservan las últimas 200 entradas; las más antiguas se eliminan.

---

# 8. Estados e indicadores

Cada estado tiene un color, un símbolo y una etiqueta. A continuación se explica qué significa cada uno y si debes actuar.

| Estado | Símbolo | Qué significa | ¿Requiere acción? |
|---|---|---|---|
| **OK / Success** | ✓ (verde) | Cuenta en línea, inicio de sesión correcto | No |
| **Running** | ▶ (azul) | La cuenta o el workflow está en marcha | No |
| **Starting** | ◐ (violeta) | Inicio en curso, estado de transición | Espera a que termine |
| **Queued** | ⏱ (gris) | Esperando en la cola | No |
| **Stopped** | ■ (gris) | Detenida, inactiva | Opcional: puedes iniciarla |
| **Paused** | ⏸ (ámbar) | Escenario pausado | Pulsa **Resume** para continuar |
| **Warning** | △ (ámbar) | Una anomalía no crítica | Mira los detalles; a menudo se puede continuar |
| **Error** | ✕ (rojo) | Un fallo recuperable | Pulsa **Retry** o investiga la causa |
| **Crashed** | ☠ (rojo oscuro, parpadea) | El proceso se cerró de forma inesperada | Pulsa **Restart** |
| **Match Found** | ◎ (verde, parpadea) | Se encontró una partida de CS2 | Nada: la aplicación confirma la disposición automáticamente |
| **Desync** | ⛓ (naranja) | Los miembros del grupo están desincronizados | Ejecuta **Re-sync** |
| **Info** | ⓘ (azul) | Un mensaje neutro | No |

**Indicadores adicionales:**

- **Recovering** (Recuperando) — un indicador azul en la barra de estado durante el arranque de la aplicación: se están recuperando los procesos de la sesión anterior. Espera a que termine.
- **Reattached** — una marca temporal en la fila de una cuenta: el proceso se recuperó correctamente tras un reinicio.
- **Frozen at HH:mm:ss** — en la pantalla **Monitoring**, significa que la visualización de datos está congelada (no en modo **Live**). Para volver a los datos en vivo, cambia a **Live** o desactiva **Freeze**.

**Cómo ver los detalles.** Pasa el cursor sobre un símbolo de estado para ver una descripción emergente: desde cuándo dura el estado, en qué paso está la cuenta y cuál fue el último evento.

![ejemplos de estados en la tabla de cuentas](../images/status-badges.png)

---

# 9. Notificaciones

La aplicación informa de los eventos de tres maneras: **avisos emergentes** (aparecen en la esquina y desaparecen), la **barra de estado** (un resumen permanente abajo) y **bandas integradas** (asociadas a una pantalla concreta).

## Avisos emergentes (Toasts)

Aparecen en la esquina inferior derecha.

| Aviso | Por qué aparece | Qué significa | Qué hacer | ¿Se puede ignorar? |
|---|---|---|---|---|
| **Saved** | Cambiaste un ajuste | El cambio se guardó | Nada | Sí, desaparece solo |
| Éxito de operación (verde) | Una acción terminó con éxito | Todo está bien | Nada | Sí, desaparece a los ~5 segundos |
| Aviso (ámbar) | Se detectó una anomalía no crítica | Merece atención | Opcionalmente, ver los detalles | Normalmente sí, desaparece a los ~10 segundos |
| Error (rojo) | Una operación falló | Requiere intervención | Pulsar **View** o **Retry** | No, permanece hasta cerrarlo a mano |
| Caída (Crash) | Un cliente se cerró de forma inesperada | Una cuenta se cayó | Pulsar **Restart** o abrir el volcado | No, permanece hasta confirmarlo |

**Conviene saber.**
- Si pasas el cursor sobre un aviso, el temporizador de auto-descarte se detiene y puedes leerlo con calma.
- Los avisos idénticos se agrupan en uno con un contador, por ejemplo `… failed (×4)`.

## Barra de estado

En el lado derecho de la barra de estado se muestra el aviso más importante sin leer, por ejemplo `● 3 errors`. Al hacer clic se abre el centro de notificaciones.

## Bandas integradas (Banners)

Aparecen en la parte superior de una pantalla y afectan al conjunto de esta. Ejemplo: `⚠ Steam network degraded — 12 accounts retrying login` (la red de Steam es inestable, 12 cuentas reintentan el inicio de sesión). Una banda se puede cerrar con el botón **Dismiss** si no es bloqueante. Las bandas bloqueantes (por ejemplo, cuando un servicio no está disponible) permanecen hasta que se resuelve el problema.

## Alertas de sonido

El sonido está desactivado por defecto. Puedes activarlo para eventos concretos (por ejemplo, **Match found** o **Crash**) en **Settings → Notifications**. Un sonido para **Match found** es útil para saber que se encontró una partida sin mirar la pantalla; la aceptación de la partida en sí ocurre de forma automática.

![un aviso de error con los botones View y Retry](../images/notification-error-toast.png)

---

# 10. Errores y solución de problemas

Los errores al operar una granja son habituales, y la aplicación te ayuda a resolverlos. A continuación tienes situaciones frecuentes en el formato «Problema → Causa posible → Solución → Resultado esperado».

## No se puede activar la licencia

**Problema.** Al introducir la clave, la aplicación no te deja continuar.

| Mensaje | Causa posible | Solución |
|---|---|---|
| «License key invalid» | La clave se introdujo con una errata | Comprueba la ortografía. Es más fácil pegar la clave con **Paste from clipboard** |
| «Used on max devices» | La licencia ya se usa en el número máximo de dispositivos | Libera la licencia en otro dispositivo y vuelve a intentarlo. El botón **Manage devices** lleva a la gestión de dispositivos |
| «Cannot reach license server» | No hay conexión con el servidor de licencias | Comprueba tu conexión a internet y pulsa **Retry** |

**Resultado esperado.** Con una clave correcta y conexión al servidor, la ventana de activación se cierra y se abre el **Dashboard**.

## Una cuenta no se inicia

**Problema.** Pulsaste **Start**, pero la cuenta no pasa a **Running**.

- **Causa posible.** La cuenta no está vinculada a una sandbox.
  **Solución.** Abre el menú contextual de la cuenta → **Bind sandbox…** y asigna una sandbox.
- **Causa posible.** Se requiere reautenticación (datos de inicio de sesión caducados); hay una marca «Reauth required» junto a la fila.
  **Solución.** Menú contextual → **Re-auth (Steam Guard)**.
- **Causa posible.** Steam ha limitado temporalmente la frecuencia de inicios de sesión.
  **Solución.** Espera alrededor de un minuto y pulsa **Retry**.

**Resultado esperado.** El estado pasa de **Starting → Running**.

## Steam se queda mucho tiempo en Waiting/Starting

**Problema.** La cuenta se atasca en la fase de inicio de sesión.

- **Causa posible.** Un inicio de sesión lento o problemas temporales de la red de Steam.
  **Solución.** Dale algo de tiempo. Si aparece un estado **Error**, pulsa **Retry**. Si la red de Steam es inestable, aparece una banda de aviso arriba; espera a que se recupere.

**Resultado esperado.** La cuenta inicia sesión y pasa a **Running**.

## Un cliente se ha caído (Crashed)

**Problema.** La cuenta obtuvo el estado **Crashed**.

- **Causa posible.** El cliente de CS2 o de Steam se cerró de forma inesperada.
  **Solución.** En la notificación que aparece, pulsa **Restart**. A menudo la recuperación ya está en marcha de forma automática. Los detalles de la caída están en la pantalla **Monitoring**, en el flujo **Crashes & Warnings**.

**Resultado esperado.** La cuenta se reinicia y vuelve a **Running**.

## Un grupo entró en Desync

**Problema.** El grupo está en el estado **Desync**: los miembros están en un estado inconsistente.

- **Causa posible.** Un miembro aceptó la partida y otro no a tiempo, o alguien salió de la cola.
  **Solución.** Pulsa **Re-sync** para pausar la cola y esperar a la consistencia. Si una cuenta causa problemas, quítala con **Drop member** y vuelve a poner al resto en cola.

**Resultado esperado.** El grupo vuelve al estado **Quorum** y está listo para la cola de nuevo.

## Un inicio masivo terminó con errores

**Problema.** Tras un **Start** masivo, algunas cuentas no se iniciaron.

- **Solución.** En el resumen, pulsa **Filter to failed**: la tabla muestra solo las cuentas problemáticas. Resuelve cada una según las causas anteriores y vuelve a iniciar.

**Resultado esperado.** Una vez resueltas las causas, un **Start** repetido lleva las cuentas a **Running**.

## Los datos de una pantalla no se cargan

**Problema.** En lugar del contenido de la pantalla, hay una banda o un mensaje de que un servicio no está disponible.

- **Causa posible.** Un servicio en segundo plano no está disponible temporalmente.
  **Solución.** Pulsa **Retry**. Si no ayuda, pulsa **Open logs** para ver los detalles, o reinicia la aplicación.

**Resultado esperado.** La pantalla se carga y muestra datos actuales.

## La aplicación informa de un proceso huérfano

**Problema.** En el centro de notificaciones, un mensaje del tipo «Orphan process … — Adopt or Kill?».

- **Causa posible.** Quedó un proceso de la sesión anterior que no se pudo vincular automáticamente a una cuenta.
  **Solución.** Elige **Adopt** (adoptarlo bajo gestión) si el proceso es necesario, o **Kill** (terminarlo) si no lo es.

**Resultado esperado.** La lista de procesos queda en orden.

## El equipo va lento y aumentan las caídas

**Problema.** Inestabilidad general, fallos frecuentes.

- **Causa posible.** Hay más cuentas en marcha de las que el equipo puede soportar.
  **Solución.** Abre **Monitoring** y mira **CPU** y **RAM**. Si los valores están cerca de sus límites, detén algunas cuentas con **Stop**.

**Resultado esperado.** La carga baja y el funcionamiento se estabiliza.

> **Códigos de error.** Los detalles de los errores incluyen un código corto como `[E-1042]`. Puedes copiarlo y usarlo al contactar con soporte. Hay una referencia completa de códigos disponible en **Help → Error reference**.

![una pantalla de error de ejemplo con los botones Retry / Open logs](../images/error-screen.png)

---

# 11. Buenas prácticas

## Preparar cuentas

- Añade las cuentas como lista con **Import**: es más rápido y hay menos erratas.
- Deja la asignación de sandbox en **Auto-assign** salvo que necesites un vínculo específico.
- Usa **Tags** para agrupar cuentas y filtrarlas rápido.

## Iniciar muchas cuentas

- Inicia por lotes: empieza con un grupo pequeño, confirma la estabilidad y luego añade más.
- Mantén el **Dashboard** o **Monitoring** abiertos para vigilar la carga en tiempo real.
- Apunta a las 4–10 cuentas de CS2 recomendadas a la vez; puedes ejecutar más en un PC potente y menos en máquinas más débiles.

## Trabajar con distribuciones

- Prepara de antemano varios preajustes para distintas situaciones (por ejemplo, «4 en stack», «uno en foco»).
- Si una distribución sale mal, usa **Revert layout** de inmediato, mientras esté activa la ventana de reversión de un minuto.

## Detener con seguridad

- Detén las cuentas con el botón **Stop** (cierre ordenado) en lugar de cerrar las ventanas a mano.
- Antes de salir de la aplicación, detén las cuentas activas. Si intentas cerrar la aplicación con escenarios en marcha, te avisa.

## Evitar interrupciones

- Antes de la cola, asegúrate de que el grupo está en el estado **Quorum**.
- Vigila las bandas sobre el estado de la red de Steam; cuando es inestable, es mejor esperar.

## Mantener un funcionamiento estable

- Consulta el **Dashboard** con regularidad: muestra el estado general en segundos.
- Mantén el número de cuentas en marcha a la vez dentro de la capacidad de tu equipo.
- Deja que la recuperación automática trabaje unos segundos antes de intervenir a mano.

---

# 12. Preguntas frecuentes

**¿Por qué no puedo iniciar una cuenta?**
Lo más probable es que la cuenta no esté vinculada a una sandbox; sin ella no se puede iniciar. Vincula una desde el menú contextual → **Bind sandbox…**. Un inicio también puede quedar bloqueado por la necesidad de reautenticar (una marca «Reauth required»); en ese caso ejecuta **Re-auth**.

**¿Por qué Steam se queda mucho tiempo en estado de espera?**
Suele ser un inicio de sesión lento o retrasos temporales de la red de Steam. Dale algo de tiempo. Si aparece un estado **Error**, pulsa **Retry**.

**¿Cómo reinicio un workflow?**
Selecciona las cuentas o instancias que necesites y pulsa **Restart** (o `Ctrl+Shift+R`). En una operación masiva, la aplicación pide confirmación.

**¿Qué pasa si la aplicación se cierra?**
Tus cuentas y ajustes están guardados. En el siguiente inicio, la aplicación intenta recuperar los procesos de la sesión anterior; aparece un indicador **Recovering** en la barra de estado. Si había escenarios activos al cerrarse, la aplicación te avisa de antemano.

**¿Cómo sé que todo funciona?**
Consulta la barra de estado de abajo y el **Dashboard**. Señales de funcionamiento normal: cuentas en estado **Running**, sin marcas rojas en la tarjeta **Errors** ni en la tabla **Failures & Crashes**, y la carga de **CPU** y **RAM** dentro de rangos normales.

**¿Dónde se guardan mis contraseñas?**
Solo en tu equipo. Se cifran con la protección integrada de Windows, nunca se guardan en texto plano y nunca se envían a ningún sitio.

**¿FarmPanel juega por mí?**
No. No es un bot ni un auto-farmeo. La aplicación gestiona el inicio, la supervisión, la formación de salas y la recuperación, mientras que todas las acciones dentro del juego las realizas tú.

**¿Hay que introducir la clave de licencia cada vez?**
No. La clave se introduce una sola vez, en la primera activación. Después la aplicación se abre directamente en el **Dashboard**.

**¿Cómo encuentro rápido una acción si no recuerdo dónde está el botón?**
Pulsa `Ctrl+K` para abrir la paleta de comandos. Empieza a escribir el nombre de una acción, una pantalla o el usuario de una cuenta, y elige el que necesites de la lista.

**¿Puedo mover la supervisión a un segundo monitor?**
Sí. En la pantalla **Monitoring**, pulsa el botón de desacoplar: la pantalla se abre como una ventana aparte que puedes colocar en un segundo monitor. Su posición se recuerda.

**¿Cómo restablezco los ajustes a sus valores por defecto?**
En **Settings → Advanced** está **Reset to defaults**. Para protegerte de clics accidentales, la aplicación pide confirmar escribiendo un texto.

---

*Fin de la guía de usuario de FarmPanel.*
