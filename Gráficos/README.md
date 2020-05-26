# Índice

- [Nvidia](#Nvidia)
   - [GeForce Experience](#GeForce-Experience)
   - [Instalación de drivers alternativa](#Instalación-de-drivers-alternativa)
   - [Configuración de vídeo](#Configuración-de-vídeo)
- [VibranceGUI](#VibranceGUI)
- [G-Sync](#G-Sync)


## Nvidia

## GeForce Experience

**Evitad instalar GeForce Experience**, en serio, evitadlo a toda costa porque añade input lag. Yo llevo años sin eso (aunque entiendo que haya gente que por temas de Praccs ya que no hay PlaysTV lo quiera usar, bueno, es inevitable) y noto que va finito, que oye, igual es placebo, pero he leído de mucha gente que ha notado input lag y yo no sé si será que iba condicionado ya o no, pero también lo notaba distinto en mi antigua 970.

Si después de ese tocho os habéis decidido a quitarlo, justo debajo tenéis una pequeña guía para hacerlo =D

## Instalación de drivers alternativa

Para este método (que os prometo que elimina input lag, 100% que no es placebo) vamos a usar un programa llamado [NVCleanstall](https://www.techpowerup.com/download/techpowerup-nvcleanstall/) para quitarle toda la "basura" a los drivers, como telemetría y características que no vamos a necesitar o están obsoletas.

Si tenéis gráficas muy antigüas no sigáis este tutorial, o si lo hacéis yo no me hago responsable, bueno, ni aunque vuestra gráfica sea modelo nuevo xD

Os recomiendo hacer un punto de restauración por si acaso algo se rompe, en mi caso no ocurrió nada y fui como un loco, pero bueno, creo que es conveniente avisarlo.

**También recomiendo desinstalar los drivers actuales con [DDU](https://www.guru3d.com/files-details/display-driver-uninstaller-download.html) (Thank Mr Laks).

1. Nos bajamos y descargamos [NVCleanstall](https://www.techpowerup.com/download/techpowerup-nvcleanstall/)
2. Una vez tenemos abierto el programa comprobamos que la casilla `Install the best driver for my hardware` está marcada (viene por defecto, pero por si aca) y le damos a Next.
3. Seleccionamos `minimum` en la parte inferior derecha, de nuevo comprobamos que todas las casillas menos la primera (que no se puede desmarcar) están DESMARCADAS.

Aquí hago un pequeño inciso antes de seguir con la guía, ya que quizá queréis usar `Shadowplay`, aunque yo no lo recomiendo, puesto que añade telemetría al sistema, tenéis que marcar la casilla. Con eso ya debería funcionar, de todos modos, si necesitáis más características aseguraos de que sean las mínimas posibles, por favor.

Repito de nuevo que yo no instalaría `Shadowplay` por muy imprescindible que fuera para mí. Si finalmente decidís instalarlo usad este [script](https://github.com/Moyster/BaiGfe) para quitar la telemetría.

4. Esperamos a que se descargue el driver.
5. Marcamos todas las casillas EXCEPTO `Unattended Express Installation`. Al marcar `Show Expert Tweaks` marcaremos también las dos nuevas opciones que aparecen `Disable NVIDIA HD Audio device sleep timer` y `Enable Message Signaled Interrupts`. Si seguís leyendo un poco más abajo encontraréis más info acerca del modo MSI.
6. Ahora se abrirá la instalación clásica (la que todos conocéis, vaya) de Nvidia.
7. Me apetecía poner el 7, ¿casualidad?

Las tarjetas gráficas normalmente funcionan (algunas vienen por defecto en MSI) en INT, al cambiarlo a MSI lo que hacemos es mejorar el tiempo de respuesta entre la CPU y la GPU. Esto significa que todo va a ser más "instant".

Con todo esto el input lag habrá desaparecido.

![alt text](https://media1.tenor.com/images/556e8f91e9b3440c007a64b93009da1d/tenor.gif "QUE TE JODAN!!!")

## Configuración de vídeo

En `Ajustar la configuración de imagen con vista previa` aka la primera opción de todas, marcaremos `Utilice la configuración avanzada de imagen 3D`.

Ahora vamos a `Controlar la configuración 3D` y dejaremos todo tal que así (si no os aparece alguna opción que a mí sí obviadla, no hay problema).

![alt text](https://i.gyazo.com/41793e89c4337bbcd01f7a8775f1238f.png "1")

![alt text](https://i.gyazo.com/037fb7356fb17269e2a149fb6bf5002f.png "2")

![alt text](https://i.gyazo.com/af7e215c25be79ffcbcca52bb91b3b48.png "3")

## VibranceGUI

VibranceGUI es una aplicación de código abierto que pone el digital vibrance a 100% solo cuando abres el programa que tú añadido. Con eso lo que conseguimos es que en el escritorio no se vea todo tan saturado pero el juego siga viéndose igual de colorido que siempre.

Con añadir el proceso al programa ya vale, luego hay que minimizarlo, no cerrarlo, y marcarle el "autostart"

[Página oficial](https://vibrancegui.com/)

## G-Sync

Si quieres informarte sobre qué es `G-Sync` [aquí puedes](https://www.nvidia.com/es-la/drivers/how-does-g-sync-work/).

Yo voy directo a la guía, para leer mi opinión bajad hasta el final.

Para tener `G-Sync` funcionando lo primero que tenemos que hacer es activarlo desde el `Panel de Nvidia`, a continuación en `Controlar la configuración 3D` activamos la `Sincronización vertical`.

Dentro de CS:GO desactivamos `Sincronización vertical`. Limita los fps con `fps_max` dependiendo de tus hz, si usas 144hz los fps deberás limitarlos por debajo, a 140, y con 240 a 235, siempre a 4-5 fps por debajo de la tasa de refresco. El objetivo del cap de fps es que al estar siempre por debajo de la tasa de refresco vais a conseguir que el `G-Sync` esté siempre activado.

Con esto reducirás el micro stuttering y lo sentirás mejor.

Mi opinión es que todo esto, salvo casos específicos de que tu PC no llegue a más fps y tengas 144hz, NO es válido, y me explico.

Esto puede llegar a añadir 1-2ms de input lag, ¿te es worth?, a mí por ejemplo no, mi PC tira perfectamente a 300fps y lo que quiero es tener el input lag al mínimo.

Salvo que estés en esa minoría que necesite activarlo recomiendo NO hacer nada de esto.
