# Índice

- [Actualizaciones de Windows](#Actualizaciones-de-Windows)
- [Plan de energía](#Plan-de-energía)
- [Teclas especiales](#Teclas-especiales)
- [Sistema modo rendimiento](#Sistema-modo-rendimiento)
- [Administración del espacio en el disco duro](#Administración-del-espacio)
- [Optimizaciones de pantalla completa](#Optimizaciones-de-pantalla-completa)
- [¿Qué versión de Windows 10 elijo?](#Windows-10)
- [Programador de tareas y Telemetría](#Programador-de-tareas-y-Telemetría)
- [Modo juego](#Modo juego)

**Os recomiendo usar el [script de Aikon](https://github.com/aikoncwd/win10script) para quitar la telemetría y toda esa mierda que viene integrada en Windows.**



## Actualizaciones de Windows

Bien, yo aquí recomiendo usar siempre [Windows 10 LTSC](https://github.com/thinkii/PC/tree/master/W10%20LTSC), si buscáis por los mares lo encontraréis. ¿Por qué? Porque trae menos mierda que el W10 normal, por poneros un ejemplo no trae ni la tienda de Windows, es decir, no podréis descargaros Netflix sin hacer una movida antes. Aparte, las actualizaciones de Windows llegan unos meses más tarde que a los Windows 10 normales, es decir, que llegan ya pulidas y sin fallos.

Una vez que tengáis eso hecho tendréis que poner en Inicio `gpedit.msc`, ya dentro iremos a `Configuración del equipo`, `Plantillas administrativas`, `Componentes de Windows`, `Windows Update` y `Configurar Actualizaciones Automáticas`.

Lo dejaremos tal que [así](https://i.gyazo.com/1324903f09075658503a69c5f1ac28dd.png). Esto impide a Windows descargar las actualizaciones por su cuenta y así no nos tocará los cojones. Cuando quieras una actualización vas tú a buscarla manualmente y la instalará porque tú quieres, nada de que haga su movida él solito.

## Plan de energía

Escribimos en inicio `Elegir un plan de energía` y elegimos `Alto rendimiento` o `Máximo rendimiento` en caso de ser posible.

Si solo os muestra el modo `Equilibrado` poned esto en el CMD `powercfg -duplicatescheme e9a42b02-d5df-448d-aa00-03f14749eb61`

## Teclas especiales 

Esto es para desactivar que se os minimicen los juegos o que se os abra una ventana al presionar 5 veces seguidas el shift

Panel de control - Accesibilidad - Centro de accesibilidad - Facilitar el uso del teclado

Y dentro desactiváis todas las casillas.

## Sistema modo rendimiento

Si tu PC es una patatilla (yo también lo tengo así y el mío no lo es) también es interesante tocar esto:

Botón derecho en Inicio, Sistema, [Información de sistema](https://i.gyazo.com/c403d3ca6c8dc0136ba0ee8d9a1b8354.png), [Configuración avanzada de sistema](https://i.gyazo.com/dd7ae324fc2f1496fe954eb966272d18.png) y hacemos clic [aquí](https://i.gyazo.com/7b191eb486cac3b4370bafb6c4ebd2e7.png).

Si lo dejáis como [esto](https://i.gyazo.com/7573895f8ac530d7c3f45ccfc18238ac.png) no notaréis diferencia más allá de la fuente, que cambiará un poquito.

## Administración del espacio

De toda la vida he instalado en C: (que suele ser el SSD) lo más importante y lo que más uso, como por ejemplo el navegador, Steam, etc.

Lo que queremos es que el CS esté a poder ser en un SSD por tema de tiempos de carga y demás, en D: (en caso de que tengáis) sería lo suyo meter los datos y todo eso, para en caso de formatear seguir con todo ahí.

## Optimizaciones de pantalla completa

La `Optimización de pantalla completa` fue añadida en la build 1607 de Windows 10 ("Anniversary Update"). Lo que hace es intentar convertir los juegos que funcionan en modo "clásico" de pantalla completa en una especie de pantalla completa sin bordes en `flip model presentation`.

### Pros

- Las optimizaciones combinan los beneficios del modo de pantalla completa con los beneficios del modo pantalla completa sin bordes, utilizando el `flip model presentation` (perdonad pero no lo he conseguido encontrar en castellano) en una ventana sin bordes maximizada.
- Disponible en aplicaciones y juegos basados en DirectX 9 o superior.

### Contras

- Puede causar problemas en algunos juegos

### Desactivar optimización de pantalla completa

En el caso de CS:GO basta con ir a la biblioteca de Steam, dar botón derecho a CS:GO, propiedades, pestaña de archivos locales, ver archivos locales y dar botón derecho a csgo.exe

Una vez ahí, elegiremos propiedades, compatibilidad, y MARCAREMOS `Deshabilitar optimizaciones de pantalla completa`.

Todo esto queda a vuestro propio criterio, ya que en algunos PCs se nota que va más fino el juego y en otros no, jugad con ese valor y dejadlo como mejor os funcione.

## Windows 10

¿Qué versión elijo?

Bueno, deciros que las diferentes versiones de Windows traen preinstaladas apps y programas que, generalmente, son mierda. Hasta ahí todo correcto, pero, ¿qué sucede? Que toda esa "mierda" estará funcionando en tu PC en segundo plano.

Es por eso por lo que queremos una versión de Windows cuyas apps, programas y servicios en segundo plano sean los mínimos posibles.

Solo faltaría que estuviéramos jugando un Faceit o un oficial y se nos pusiera a actualizar algunos de esos programas inútiles en 2º plano y nos diera un pantallazo azul.

- Evitad cualquier build de Preview o Insider
- Evitar ediciones Pro o Home
- Usad Education (Enterprise) o versiones LTSC (si es posible)

## Programador de tareas y Telemetría

Aquí os dejo una lista de tareas a desactivar (afectan a privacidad y rendimiento)

- \Microsoft\Windows\Application Experience > AitAgent, ProgramDataUpdater
- \Microsoft\Windows\Autochk > Proxy
- \Microsoft\Windows\Customer Experience Improvement Program> Consolidator, KernelCeipTask, UsbCeip
- \Microsoft\Windows\DiskDiagnostic > Microsoft-Windows-DiskDiagnosticDataCollector
- \Microsoft\Windows\Maintenance > WinSAT
- \Microsoft\cSystemRestore > SR
- \Microsoft\Windows\WindowsBackup > ConfigNotification
- \Microsoft\Windows Defender > MP Scheduled Scan
- \Library\Microsoft\Windows\WindowsColorSystem\Calibration Loader (disable it if you use your own Display Color Profile)
- \Microsoft\Microsoft\CDPUserSvc

Copia el contenido del [siguiente archivo](https://github.com/thinkii/PC/blob/master/Misc/antitelemtry.cmd) en un txt y pone este nombre `antitelemetry.cmd`

Ejecútalo para desactivar las cosillas de telemetría (si lo has hecho con el script de Aikon esto es inútil, porque ya lo hiciste antes). Si por otro lado quieres asegurarte de que siempre va a estar todo bloqueado puedes crear una tarea para que se ejecute siempre que inicies Windows y así te curas en salud.

1. Copia el archivo en `C:\Windows` y ejecuta CMD como administrador.
2. SCHTASKS /Create /F /RU "SYSTEM" /RL HIGHEST /SC ONSTART /TN BlockW10 /TR "cmd /c %windir%\antitelemetry.cmd"


## Modo juego

El [modo juego](https://beta.support.xbox.com/help/games-apps/game-setup-and-play/use-game-mode-gaming-on-pc) permite al sistema priorizar los recursos de CPU y GPU al juego que se está ejecutando en primer plano, y su objetivo es garantizar un aumento de fps, o por lo menos picos más altos, junto a un aumento de la media de fps y su consistencia. En las últimas versiones de Windows, comenzando con la Build 1809 y 1903, el Modo juego ya no prioriza la GPU/CPU. Esto significa que los procesos en segundo plano reciben más recursos en caso de que otras aplicaciones (OBS por ejemplo) requieran de muchos, en este caso debido al encoding. 

- Activar el `Modo juego` evita que Windows Update actualice drivers y desactiva las notificaciones de actualizaciones que no sean muy importantes.

- Fuerza (si está activado) un uso mínimo del 100% de la CPU en ordenadores de sobremesa (en portátiles no), para ayudar a reducir las fluctuaciones que pueden convertirse en problemas de rendimiento. Hace exactamente lo mismo que ir a la administración de potencia del procesador y poner el estado mínimo del procesador en 100% (plan de energía de `Alto rendimiento`)

- El modo juego no viene activado por defecto, esto se basa en la versión que utilicéis de Windows. De la 1809 en adelante el juego puede decidir si activar ese `Modo juego` o no.

- El `Modo juego` se comporta de manera diferente en portátiles para evitar problemas de sobrecalentamiento.

Dicho todo esto, en versiones superiores a 1903 el `Modo juego` NO afecta negativamente al rendimiento de los juegos.
