Os recomiendo usar el [script de Aikon](https://github.com/aikoncwd/win10script) para quitar la telemetría y toda esa mierda que viene integrada en Windows.

> Actualizaciones de Windows

Bien, yo aquí recomiendo usar siempre [Windows 10 LTSC](https://github.com/thinkii/PC/tree/master/W10%20LTSC), si buscáis por los mares lo encontraréis. ¿Por qué? Porque trae menos mierda que el W10 normal, por poneros un ejemplo no trae ni la tienda de Windows, es decir, no podréis descargaros Netflix sin hacer una movida antes. Aparte, las actualizaciones de Windows llegan unos meses más tarde que a los Windows 10 normales, es decir, que llegan ya pulidas y sin fallos.

Una vez que tengáis eso hecho tendréis que poner en Inicio `gpedit.msc`, ya dentro iremos a `Configuración del equipo`, `Plantillas administrativas`, `Componentes de Windows`, `Windows Update` y `Configurar Actualizaciones Automáticas`.

Lo dejaremos tal que [así](https://i.gyazo.com/1324903f09075658503a69c5f1ac28dd.png). Esto impide a Windows descargar las actualizaciones por su cuenta y así no nos tocará los cojones. Cuando quieras una actualización vas tú a buscarla manualmente y la instalará porque tú quieres, nada de que haga su movida él solito.

> Plan de energía

Escribimos en inicio `Elegir un plan de energía` y elegimos `Alto rendimiento` o `Máximo rendimiento` en caso de ser posible.

Si solo os muestra el modo `Equilibrado` poned esto en el CMD `powercfg -duplicatescheme e9a42b02-d5df-448d-aa00-03f14749eb61`

> Teclas especiales 

Esto es para desactivar que se os minimicen los juegos o que se os abra una ventana al presionar 5 veces seguidas el shift

Panel de control - Accesibilidad - Centro de accesibilidad - Facilitar el uso del teclado

Y dentro desactiváis todas las casillas.

> Sistema - Rendimiento

Si tu PC es una patatilla (yo también lo tengo así y el mío no lo es) también es interesante tocar esto:

Botón derecho en Inicio, Sistema, [Información de sistema](https://i.gyazo.com/c403d3ca6c8dc0136ba0ee8d9a1b8354.png), [Configuración avanzada de sistema](https://i.gyazo.com/dd7ae324fc2f1496fe954eb966272d18.png) y hacemos clic [aquí](https://i.gyazo.com/7b191eb486cac3b4370bafb6c4ebd2e7.png).

Si lo dejáis como [esto](https://i.gyazo.com/7573895f8ac530d7c3f45ccfc18238ac.png) no notaréis diferencia más allá de la fuente, que cambiará un poquito.
