# Índice

- [Nvidia](#Nvidia)
   - [GeForce Experience](#GeForce-Experience)
   - [Descarga](#Descarga)
- [VibranceGUI](#VibranceGUI)
- [G-Sync](#G-Sync)


## Nvidia

Aquí hay poco tema, básicamente yo de toda la vida he usado el modo rendimiento.

![alt text](https://i.gyazo.com/e23a8f037c5c1cd463eb30a218f7a788.png "Modo rendimiento de tarjeta gráfica")

Pero desde que metieron el `Low Latency Mode` entiendo que haya gente que use la **configuración avanzada de 3D**.

Dentro de la **configuración avanzada de 3D** lo único que os puedo decir que toquéis es el `Low Latency Mode` a Ultra y que lo testeéis, ya que no a todo el mundo le va bien y que el `Modo de control de energía` lo pongáis al máximo.

Añadir también que no soy fan del G-Sync, no me gusta, pero sois libres de hacer lo que queráis.

## GeForce Experience

Una vez dicho todo esto, **evitad instalar GeForce Experience**, en serio, evitadlo a toda costa porque añade input lag. Yo llevo años sin eso (aunque entiendo que haya gente que por temas de Praccs ya que no hay PlaysTV lo quiera usar, bueno, es inevitable) y noto que va finito, que oye, igual es placebo, pero he leído de mucha gente que ha notado input lag y yo no sé si será que iba condicionado ya o no, pero también lo notaba distinto en mi antigua 970.

## Descarga

Podéis descargar los últimos drivers desde la [página oficial](https://www.nvidia.com/Download/index.aspx)

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
