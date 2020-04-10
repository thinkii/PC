# Índice

- [TeamSpeak](#TeamSpeak)
- [Drivers de sonido](#Drivers-de-sonido)
- [Actualizar Realtek](#Actualizar-Realtek)

## Primeros pasos en Windows recién instalado

Lo primero que queremos hacer nada más arrancar Windows por primera vez es cambiar las comunicaciones a `No hacer nada`

Para ello le damos botón derecho al iconito de la barra del altavoz y elegimos `Sonidos`, luego basta con dejarlo [así](https://i.gyazo.com/2d36797c54fd3f9ca81936b60fc07626.png)

Después, en la misma ventana, iremos a `Reproducción` y elegiremos nuestro dispositivo, iremos a `Enhancements` y marcaremos `Loudness Equalization`, esto lo que hace es que los pasos y disparos en CS:GO se oigan por igual, esto mejora el sonido de los pasos dentro la partida. Si llevas mucho tiempo con esto desactivado te costará un poquito acostumbrarte.

**Si CS:GO saca alguna actualización de sonido en la que se emule de alguna manera esto o se equilibre el sonido de los pasos con los disparos, volved y desactivad esto**

Por último iremos a la pestaña `Opciones avanzadas` y elegiremos [esta opción](https://i.gyazo.com/c4942a566a415b92932fe7cfbb462f8a.png) en cuanto a calidad de sonido se refiere. En algunos sitios recomiendan 44100 Hz pero a mí la que mejor me ha ido siempre ha sido esta (48000 Hz), nunca me ha dado ningún problema.

Si no tenéis un PC muy potente dejadlo en 44100 Hz, porque el salto de calidad de 44100 a 48000 es tan mínimo que es imperceptible, y puede provocar una ligera carga extra en vuestra CPU. En la gran mayoría de los casos si queréis 48000 estáis bien, no os preocupéis.

## TeamSpeak

Me voy a fumar un señor puro y voy a meter TeamSpeak aquí, os recomiendo que os creéis una cuenta de MyTeamSpeak, así se os sincronizará vuestra cuenta (admins en diferentes servidores de TS, los servidores que tengáis en marcadores, etc.) con MyTeamSpeak y al formatear todo no perderéis nada.

Os sorprendería la cantidad de gente que no tiene cuenta de MyTeamSpeak en pleno 2020.

[Link de descarga](https://www.teamspeak.com/es/downloads/)

PD: Ya de paso os dejo un código de insignia que no caduca, como premio porque os hayáis creado la cuenta jaja `RWGE2NURJZ`

Se canjea [aquí](https://i.gyazo.com/af1bec68a8b18aa990312f54a233c823.png)

## Drivers de sonido

Aunque os parezca mentira, hace años leí en reddit que un usuario reportaba que al actualizar los drivers de Realtek le subió el rendimiento en CS una pasada, pero en tema de fluidez. Yo no me lo creía, pero lo probé y sí, era verdad (la razón por la que esto sucedía no la recuerdo, para qué os voy a mentir).

Así que buscad actualizaciones regularmente.

## Actualizar Realtek

Para actualizar Realtek vamos a [esta página](https://www.tenforums.com/sound-audio/135259-latest-realtek-hd-audio-driver-version-2-a.html) que recoge los últimos drivers (son jodidos de encontrar, creedme), lo descargáis de la derecha, dándole a descargar. Una vez descargado, guardad el .zip en una carpeta vacía en el escritorio por ejemplo, y descomprimidla.

Luego seguid los pasos de [este tutorial](https://www.tenforums.com/tutorials/66346-install-cab-file-windows-10-a.html#post873775). Escribís en inicio `Administrador de dispositivos` y buscáis `Controladora de sonido y vídeo y dispositivos de juego` y el resto aunque no sepáis inglés lo vais a entender perfectamente en el tutorial.
