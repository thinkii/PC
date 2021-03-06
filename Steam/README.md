# Índice

- [Parámetros](#Parámetros)
- [Biblioteca](#Biblioteca)
   - [Opciones de lanzamiento](#Opciones-de-lanzamiento)
- [Precarga de sombreadores](#Precarga-de-sombreadores)

En Steam lo primero que hago nada más formatear es ir a parámetros y dejar todo así

## Parámetros

- Interfaz

![alt text](https://i.gyazo.com/dc7aa0be04c8652fa13d3cff78551a14.png "Interfaz")

- Preferencias de barra de tareas

![alt text](https://i.gyazo.com/07331db8b76f25dfa1324cad84f4fa6c.png "Preferencias de barra de tareas")

- Chat-Lista de amigos

![alt text](https://i.gyazo.com/340b77465a62dc38cb8b44aac5c77352.png "Chat-Lista de amigos")

- Chat-Notificaciones

![alt text](https://i.gyazo.com/ec3f044db1e7da48e85184c66a51644b.png "Chat-Notificaciones")

## Biblioteca

- Las dos opciones de abajo tienen que ir en `Desactivación forzosa`

![alt text](https://i.gyazo.com/4a246c87cbb6fa21c93868fd6339d6b3.png "Desactivación forzosa")

- Tampoco queremos que descargue actualizaciones de otros juegos en segundo plano, aunque esto juraría que viene por defecto bien.

![alt text](https://i.gyazo.com/d8d28d9226218b9a41ee444c0907ff2e.png "Descargas en segundo plano")

## Opciones de lanzamiento

Un desarrollador de Valve dijo en reddit que las mejores opciones de lanzamiento es no tener, así que vamos a intentar poner las menores posibles.

Dentro de las más útiles yo metería `-novid`, `-high` (solo si tu PC es bueno, si tienes un PC normalito o patatilla puede causar más problemas que beneficios) y `-tickrate 128`

Mención especial a `+clientport XXXXX` que nos salva de muchos problemas especialmente en Faceit. 

Su funcionamiento es sencillo, si la IP a la que te vas a conectar es esta por ejemplo: XX.XXX.XXX.XX:20020 pondremos en opciones de lanzamiento `+clientport 20020`, pero solo si entramos al servidor previamente y tenemos loss o mucho ping por bad routing.

## Precarga de sombreadores

Es bastante posible que cuando salga Source 2 (lo que implica la llegada de Vulkan también) queramos tener activado este ajuste. De momento lo dejaremos desmarcado.

