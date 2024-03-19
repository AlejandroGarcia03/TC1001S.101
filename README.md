# TC1001S.101
Archivos de Herramientas computacionales: el arte de la programación
### Cristian Alejandro García Mendoza
### IRS
### Irapuato
# Encabezados
Para crear un encabezado, agrega uno a seis símbolos # antes del encabezado del texto.
# Encabezado grande   Cristian Alejandro García Mendoza
## Encabezado mediano Cristian Alejandro García Mendoza
### Encabezado pequeño Cristian Alejandro García Mendoza
### Encabezado pequeñito Cristian Alejandro García Mendoza
#### Encabezado diminuto Cristian Alejandro García Mendoza
##### Encabezado mini Cristian Alejandro García Mendoza
###### Encabezado micro Cristian Alejandro García Mendoza


# Guía de MarkDown
[link a guía](https://www.markdownguide.org/cheat-sheet/)
Puedes indicar énfasis con texto en negritas, itálicas o tachadas en los campos de comentario y archivos .md

#Estilo
- Negrita **** **Este texto está en negrita**
-Cursiva "" o -- --*Este texto está en cursiva* y _este también_
- Tachado ~~ ~~ ~~{Este texto está equivocado~~
-Cursiva en negrita y anidada ** y _ **Este_texto_es_extremadamente_importante**
-Todo en negrita y cursiva *** ***  ***Todo este texto es importante***
I
# Usar emojis inicia escribiendo + letra escoges el emoji que quieres
🥇
🇲🇽
🎾
🤖
♓
# Tabla
| Tabla | Syntax 2 | Description 3 |
| ------------ | ------------ | ------------ |
| Dato 1       | Dato 2       | Dato 3       |
| Dato 4       | Dato 5       | Dato 6       |

#Cita de Texto
> ITESM
# Enlace
[GitHub Pages] (https://pages.github.com/)
# Imagen
![GitHub Pages] (https://www.irapuatoguanajuato.com.mx/wp-content/uploads/2014/01/escudo_ciudad_de_irapuato_guanajuato_mexico_significado_colores_historia_fundacion_bandera_00.jpg)


``` geojson
{
"type": "Polygon",
  "coordinates" : [
    [
      [-85, 35],
      [-100.2155, 25.6748],
      [-100.309, 25.6714], 
      [-101.35628, 20.67675],
      [-85,30]
    ]
  ]
}
```
![GitHub Brillante] (https://tec.mx/sites/default/files/styles/header_full/public/2018-12/FachadaTec_0.jpg?itok=_HoeD7qc)
# Listas
Puedes realizar una lista desordenada al anteceder una o más líneas de texto con
-Panda Rojo
-Ron da error
- Los Picapiedra
1. Panda Rojo 2. Ron da error 3. Los Picapiedra
# Listas Anidadas Primer Concierto 
- Primer concierto
- Primer pijamada
  - Panda
# Lista de Tareas
- [x]  Alejandro García 
- [] Cesar Alejandro Benavides
- [] Rodrigo Ibarra
# Ocultar el contenido
<!-- This content will not appear in the rendered Markdown -->

| Syntax | Description |
| Header | Title |
| Paragraph | Text |

```
{
"firstName": "John",
"lastName": "Smith", 
"age": 25,
}
```

# Código
```from turtle import *

from freegames import vector


def line(start, end):
    """Draw line from start to end."""
    up()
    goto(start.x, start.y)
    down()
    goto(end.x, end.y)


def square(start, end):
    """Draw square from start to end."""
    up()
    goto(start.x, start.y)
    down()
    begin_fill()

    for count in range(4):
        forward(end.x - start.x)
        left(90)

    end_fill()


def circle(start, end):
    """Draw circle from start to end."""
    pass  # TODO


def rectangle(start, end):
    """Draw rectangle from start to end."""
    pass  # TODO


def triangle(start, end):
    """Draw triangle from start to end."""
    pass  # TODO


def tap(x, y):
    """Store starting point or draw shape."""
    start = state['start']

    if start is None:
        state['start'] = vector(x, y)
    else:
        shape = state['shape']
        end = vector(x, y)
        shape(start, end)
        state['start'] = None


def store(key, value):
    """Store value in state at key."""
    state[key] = value


state = {'start': None, 'shape': line}
setup(420, 420, 370, 0)
onscreenclick(tap)
listen()
onkey(undo, 'u')
onkey(lambda: color('black'), 'K')
onkey(lambda: color('white'), 'W')
onkey(lambda: color('green'), 'G')
onkey(lambda: color('blue'), 'B')
onkey(lambda: color('red'), 'R')
onkey(lambda: store('shape', line), 'l')
onkey(lambda: store('shape', square), 's')
onkey(lambda: store('shape', circle), 'c')
onkey(lambda: store('shape', rectangle), 'r')
onkey(lambda: store('shape', triangle), 't')
done()
Logo

Free Python Games


Donate
If you or your organization uses Free Games, consider donating:

Donate to Free Python Games

Related Topics
Documentation overview
Previous: Illusion
Next: Maze
Quick search
```
