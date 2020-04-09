# Tabla de contenido

- [Sensibilidad](#Sensibilidad)
- [Aceleración 1.0](#Aceleración-1.0)
- [DPI](#DPI)
- [Hz del ratón](#Hz-del-ratón)
- [Aceleración 2.0](#Aceleración-2.0)

## Sensibilidad

La sensibilidad de Windows se deja siempre en 6/11, si no me equivoco es la que viene por defecto.

## Aceleración 1.0

Aunque dentro de CS:GO vayamos a usar el `m_rawinput "1"`, yo siempre desactivo la aceleración desde Windows "por si aca".

Para ello escribiremos `Mouse` en inicio y nos abrirá algo como [esto](https://i.gyazo.com/73d032a9448dfc4846682e9d893f5dfd.png). Iremos a `Opciones de mouse adicionales`, `Opciones de puntero` y desmarcaremos [Mejorar precisión de puntero](https://i.gyazo.com/b4edcb6c34b4d118c35d247d9c339479.png)

Recomiendo también de vez en cuando coger un bastoncillo, darle alcohol y limpiar el sensor con cuidado con él, sin hacer mucha fuerza.

Y con la alfombrilla más de lo mismo, de vez en cuando una lavadita no le viene mal, que se acumula la mierda que da miedo.

## DPI

Yo los llevo a 800 desde hace muchos años, los DPI son la cantidad de puntos que recorre el puntero por pulgada.

Pienso que el equilibrio está en 800, 400 es poco y a 800 se nota algo de mejoría.

## Hz del ratón

Recomiendo tenerlos a 1000 o como muy poco 500, yo si lo tengo a menos noto que no va fluido del todo.

## Aceleración 2.0

Hay veces que no se desactiva bien la aceleración desde el panel de control, así que lo más seguro es hacerlo desde el registro

En inicio escribimos **regedit** y lo ejecutamos como administrador. Vamos a `HKEY_CURRENT_USER\Control Panel\Mouse` y editamos las dos entradas `SmoothMouseXCurve` y `SmoothMouseYCurve`

Lo dejamos tal que así

    SmoothMouseXCurve

    00,00,00,00,00,00,00,00
    00,a0,00,00,00,00,00,00
    00,40,01,00,00,00,00,00
    00,80,02,00,00,00,00,00
    00,00,05,00,00,00,00,00


    SmoothMouseYCurve

    00,00,00,00,00,00,00,00
    66,a6,02,00,00,00,00,00
    cd,4c,05,00,00,00,00,00
    a0,99,0a,00,00,00,00,00
    38,33,15,00,00,00,00,00
