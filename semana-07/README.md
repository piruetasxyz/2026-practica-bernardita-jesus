# Semana-07

## Resumen de días, temas y horas

| Fecha      | Día      | Temas                                                | Lugar     | Horas día / hora semana |
| :--------- | :------- | :--------------------------------------------------- | :-------- | :---------------------- |
| 2026-08-31 | Lunes    | Investigación de elementos, Impresión 3D             | LID       | 008 / 008               |
| 2026-09-01 | Martes   | Impresión 3D                                         | República 180 | 003 / 011               |
| 2026-09-03 | Jueves   |                                                      |           | 000 / 000               |
| 2026-09-04 | Viernes  |                                                      |           | 000 / 000               |
| 2026-09-05 | Sábado   |                                                      |           | 000 / 000               |
| 2026-09-06 | Domingo  |                                                      |           | 000 / 000               |

## Correcciones Paneles

### Elementos para los paneles

Los elementos y piezas externas principales de los paneles son M3, entradas jacks, potenciómetros y LEDs, pero para ver la viabilidad del modelado, lo más importante son las medidas de los potenciómetros, que en el código están clasificados como perillas y jacks.

#### Perillas

Respecto a las perillas, y navegando en [Thonk](thonk.co.uk), me di cuenta de que se montan sobre el mismo potenciómetro y que lo que varía es solo la tapa, con la que se interactúa. Por tanto, en el código de las variables comunes, de esa misma carpeta, que es donde conviven las funciones de las que se referencian todas las medidas de los paneles, lo modifiqué y ahora solo existe una perilla, con un tamaño igual. Antes existían perillas pequeñas, medianas y grandes.

https://www.thonk.co.uk/shop/intellijel-white-knobs/

Bueno, y no solo por un hecho funcional. Yo creo que realmente sería incompatible utilizar perillas que sobrepasen el diámetro de 10 mm.

#### Jacks TS de 3,5 mm

Por el lado de las entradas y salidas, los jacks TS de 3,5 mm son piezas que, en el fondo, tienen un cilindro con una rosca que atraviesa la perforación del panel y luego se ajusta con una tuerca. En las pruebas de la versión 0.0.6, estas piezas quedaban un poco ajustadas, por lo que fui ajustando las medidas a través de un proceso de iteración.

En estas mismas pruebas determiné que, en los módulos de 4 HP, donde existen dos columnas de grilla, no es posible tener dos jacks uno al lado del otro, o al menos no sin dejar una mayor distancia entre ellos y un margen que resulta preocupantemente reducido y endeble, dependiendo del material.

Adjuntar foto de cómo topan las piezas de los jacks*

Esta imposibilidad la desarrollaré en el siguiente tema.

#### Potenciómetros

Agregando a esto, a mi criterio, me parece una buena idea utilizar potenciómetros tipo D, ya que permiten fabricar con mayor facilidad perillas y tapas custom, sin que se desgaste el material en exceso. Esto se debe a que tienen un encaje que no posee un eje de simetría, lo que permite dejar una posición estática de la perilla en el potenciómetro, y el giro no produciría un desgaste excesivo del material.

https://www.thonk.co.uk/shop/alpha-9mm-pots-dshaft/

### Nuevas medidas de los paneles

Como mencioné, antes los paneles los estábamos desarrollando en dos medidas, estandarizadas por el formato Eurorack, en HP, lo que quiere decir Horizontal Pitch. En este formato, cada HP corresponde a 5,08 mm de ancho, por lo que:

|    HP | Ancho (mm) |
| ----: | ---------: |
|  1 HP |    5,08 mm |
|  2 HP |   10,16 mm |
|  3 HP |   15,24 mm |
|  4 HP |   20,32 mm |
|  5 HP |   25,40 mm |
|  6 HP |   30,48 mm |
|  7 HP |   35,56 mm |
|  8 HP |   40,64 mm |
|  9 HP |   45,72 mm |
| 10 HP |   50,80 mm |

Ya que en las pruebas con los elementos no podían montarse sobre los paneles de 4 HP dos entradas o salidas de jacks TS de 3,5 mm una al lado de la otra, decidí cambiar las medidas de los paneles a 5 HP y 10 HP.

## Escáner

https://structure.io/

nos escaneamos para la pagina web

Link de Aarón y Mateo rebotando*

https://piruetas.xyz/rebotar.html

## Salidas

### Museo Violeta Parra
