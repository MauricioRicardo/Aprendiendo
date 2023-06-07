# Markdown Sintaxis
En este espacio es para tener a la mano la sintaxis de los diferentes comandos con sus variables y sus diferentes formas de realizar la misma acción

<!-- HEADINGS -->
## Encabezados
```
# Encabezado Tamaño 1
## Encabezado Tamaño 2
### Encabezado Tamaño 3
#### Encabezado Tamaño 4
##### Encabezado Tamaño 5

Una alternativa para los Headers de tamaño 1 y 2 con subrayado es:
Alternativa Encabezado Tamaño 1
=
Alternativa Encabezado Tamaño 2
-
```
# Encabezado Tamaño 1
## Encabezado Tamaño 2
### Encabezado Tamaño 3
#### Encabezado Tamaño 4
##### Encabezado Tamaño 5

Una alternativa para los Headers de tamaño 1 y 2 con subrayado es:

Alternativa Encabezado Tamaño 1
=
Alternativa Encabezado Tamaño 2
-
---
<!-- CURSIVA - NEGRITAS - TACHADO -->
## Estilos de Texto
```
Para indicar énfasis con *Cursiva*, es con *asteriscos* o _guiones bajos_ 
Para indicar énfasis con **Negrita**, es con dos **asterisco** o __guiones bajos__
Para indicar énfasis combinado, es con **asteriscos y _guiones bajos_**
Para indicar énfasis con <sub>subíndice</sub> es con la etiqueta <sub>sub</sub>
Para indicar énfasis con <sup>superíndice</sup> es con la etiqueta <sup>sup</sup>
Para tachar el texto es con dos ~~virgulillas~~
```
Para indicar énfasis con *Cursiva*, es con *asteriscos* o _guiones bajos_ 

Para indicar énfasis con **Negrita**, es con dos **asterisco** o __guiones bajos__

Para indicar énfasis combinado, es con **asteriscos y _guiones bajos_**

Para indicar énfasis con <sub>subíndice</sub> es con la etiqueta <sub>sub</sub>

Para indicar énfasis con <sup>superíndice</sup> es con la etiqueta <sup>sup</sup>

Para tachar el texto es con dos ~~virgulillas~~
___
<!-- LISTA DESORDENADA -->
## Lista Ordenada
```
1. Primer elemento de una lista ordena
2. Segundo elemento de una lista ordena
9. El valor del número no importa, con que solo sea un numero
    1. Sub lista ordenado
    5. Sub lista con número que no consecutivo del anterior
7. Otro elemento
    Para tener un párrafo de texto con sangría dentro de una lista, solo tenemos que precionar la tecla de tabulador (TAB)
```
1. Primer elemento de una lista ordena
2. Segundo elemento de una lista ordena
9. El valor del número no importa, con que solo sea un numero
    1. Sub lista ordenado
    5. Sub lista con número que no consecutivo del anterior
7. Otro elemento  
    Para tener un párrafo de texto con sangría dentro de una lista, solo tenemos que precionar la tecla de tabulador (TAB)
___
<!-- LISTA ORDENADA -->
## Lista Desordenada
```
* La lista desordenada puedes usar asterisco
    * Sub lista desordena
        * Sub lista de la sub lista anterior
- También puedes utilizar un menos
    + También puedes utilizar el mas
        * O combinar las tres formas anteriores
```
* La lista desordenada puedes usar asterisco
    * Sub lista desordena
        * Sub lista de la sub lista anterior
- También puedes utilizar un menos
    + También puedes utilizar el mas
        * O combinar las tres formas anteriores
___
<!-- ENLASE -->
## Enlaces
Para realizar enlaces hay dos formas relativas (Dentro del proyecto) y absolutas (Fuera del proyecto)
```
[Enlace absoluto en línea](https://www.youtube.com/)

[Enlace absoluto en línea con título](https://www.youtube.com/ "Página principal de YouTube")

[Enlace absoluto con referencia][El texto de referencia debe ser insensitive para no tener problemas con el enlace]

[Enlace relativo con referencia a un archivo del repositorio](./Recursos/Luffy.md)

[También se puede utilizar números para definir el enlace absoluto de referencia][1]

o podemos dejar vacío y utilizar el [texto del enlace]

[El texto de referencia debe ser insensitive para no tener problemas con el enlace]: https://www.mozilla.org
[1]: /www.google.com
[texto del enlace]: http://www.reddit.com 
```

[Enlace absoluto en línea](https://www.youtube.com/)

[Enlace absoluto en línea con título](https://www.youtube.com/ "Página principal de YouTube")

[Enlace absoluto con referencia][El texto de referencia debe ser insensitive para no tener problemas con el enlace]

[Enlace relativo con referencia a un archivo del repositorio](./Recursos/Luffy.md)

[También se puede utilizar números para definir el enlace absoluto de referencia][1]

o podemos dejar vacío y utilizar el [texto del enlace]

[El texto de referencia debe ser insensitive para no tener problemas con el enlace]: https://www.mozilla.org
[1]: https://www.google.com
[texto del enlace]: http://www.reddit.com 
___
<!-- IMAGENES -->
## Imagenes
```
El logo de Pi (Al pasar el cursor sobre el logo mostrara un título)
Imagen en línea:
![Pi]
(https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")

Imagen referenciada de nuestro proyecto:
![PI](https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")

Imagen que cambia dependiendo el tema que tengamos en nuestro equipo en caso de que el tema sea oscuro se mostrar una luna en caso de que el tema sea claro se mostrara una sol

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/Luna_gzuafj.png">

  <source media="(prefers-color-scheme: light)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/sol_lxxaqy.png">
  
  <img alt="Muestra un sol en modos claras y una luna con modos oscuros" src="https://res.cloudinary.com/dtzgksveo/image/upload/v1686090395/PitooPlumo/Eclipse_c3zooy.png">
</picture>
```
El logo de Pi (Al pasar el cursor sobre el logo muestra un titulo)

Imagen en linea:
![Pi](https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")

Imegen referenciada de nuestro proyecto:
![PI](./Recursos/Pi.png "Logo de Pi")

Imagen que cambia dependiendo el tema que tengamos en nuestro equipo en caso de que el tema sea oscuro se mostrar una luna en caso de que el tema sea claro se mostrara una sol

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/Luna_gzuafj.png">

  <source media="(prefers-color-scheme: light)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/sol_lxxaqy.png">
  
  <img alt="Muestra un sol en modos claras y una luna con modos osucros" src="https://res.cloudinary.com/dtzgksveo/image/upload/v1686090395/PitooPlumo/Eclipse_c3zooy.png">
</picture>

___
<!-- BLOQUE DE CODIGO -->
## Código 
Los bloques de código forman parte de la especificación de Markdown, pero el resaltado de sintaxis no. Sin embargo, muchos renderizados, como GitHub lo soportan

```
El `código` que quieras resaltar como código al su alrededor tiene acento `grave`
```
El `código` que quieras resaltar al su alrededor tiene `acento grave`

Los bloques de código están  delimitados por tres acentos graves ` ``` `

```
 ```javascript 
Syntaxis de JavaScrip
import axios from 'axios';
import { defineStore } from 'pinia';
import login from '../services/login.js';
export const useLoginStore = defineStore('login', {
    state: () => ({
        email: "",
    }),   
    }
});
    ```
```
```javascript 
Syntaxis de JavaScrip
import axios from 'axios';
import { defineStore } from 'pinia';
import login from '../services/login.js';
export const useLoginStore = defineStore('login', {
    state: () => ({
        email: "",
    }),   
    }
});
```
---
## Codigo HTML
También se puede utilizar código HTML sin formato y la mayoría de las funciones se pueden utilizar
```
<dl>
  <dt>Lista de Definiciones</dt>
  <dd>Algunas personas utilizan HTML</dd>

  <dt>Mackdown en HTML</dt>
  <dd>No **funciona** *nada* `bien`. Usa <em>etiquetas</em> HTML</dd>
</dl>
```
<dl>
  <dt>Lista de Definiciones</dt>
  <dd>Algunas personas utilizan HTML</dd>

  <dt>Mackdown en HTML</dt>
  <dd>No **funciona** *nada* `bien`. Usa <em>etiquetas</em> HTML</dd>
</dl>

___
## Nota a Pie de Página
Las notas no forman parte de la especificación de Markdown, pero son soportadas por GitHub
```
Esto es unas notas simples[^1]

Una nota también puede tener varias líneas[^2]

También se puede utilizar palabras, para la referencia[^nota]

[^1]: Mi referencia

[^2]: Cada nueva línea debe ir antes dos espacios
 Esto permite tener una nota con varias líneas

 [^nota]:
    Las notas con nombre seguirán mostrando números en lugar de texto, pero permiten una mejor identificación y un enlace más sencillo.
    Esta nota también se ha hecho con una sintaxis diferente utilizando cuatro espacios para las nuevas líneas.

```
Esto es unas notas simples[^1]

Una nota también puede tener varias líneas[^2]

También se puede utilizar palabras, para la referencia[^nota]

[^1]: Mi referencia

[^2]: Cada nueva línea debe ir antes dos espacios
 Esto permite tener una nota con varias líneas

 [^nota]:
    Las notas con nombre seguirán mostrando números en lugar de texto, pero permiten una mejor identificación y un enlace más sencillo.
    Esta nota también se ha hecho con una sintaxis diferente utilizando cuatro espacios para las nuevas líneas.
___
<!-- TABLAS -->
## Tabla
Las tablas no forman parte de las especificaciones de Markdown, pero GitHub las soporta
```
Se puede utilizar dos puntos para alinear las columnas

|    Carro   |  Color  |   Modelo  |  Año  |
|------------|:-------:|----------:|-------|
| Celica     | Negro   | GTS       | 2006  |
| Honda      | Azul    | Civic     | 2001  |
| Tesla      | Blanco  | S         | 2020  |
| Land Rover | Gris    | Defender  | 2023  |
| Lincoln    | Dorado  | Navigator | 2020  |

Debe haber al menos tres guiones para realizar la cabecera.
Las plecas (|) del exterior son opcionales y no es necesario para realizar la tabla igual que la alineación no es necesaria. Dentro de las columnas también se pueden utilizar los comandos para destacar cierto texto

Normal|Cursiva|Negrita|Código|Tachado
---|---|---|---|---|
Markdown|*Markdown*|**Markdown**|`Markdown`|~~Markdown~~
1|*2*|**3**|`4`|~~5~~
```
Se puede utilizar dos puntos para alinear las columnas

|    Carro   |  Color  |   Modelo  |  Año  |
|------------|:-------:|----------:|-------|
| Celica     | Negro   | GTS       | 2006  |
| Honda      | Azul    | Civic     | 2001  |
| Tesla      | Blanco  | S         | 2020  |
| Land Rover | Gris    | Defender  | 2023  |
| Lincoln    | Dorado  | Navigator | 2020  |

Debe haber al menos tres guiones para realizar la cabecera.
Las plecas (|) del exterior son opcionales y no es necesario para realizar la tabla igual que la alineación no es necesaria. Dentro de las columnas también se pueden utilizar los comandos para destacar cierto texto

Normal|Cursiva|Negrita|Código|Tachado
---|---|---|---|---|
Markdown|*Markdown*|**Markdown**|`Markdown`|~~Markdown~~
1|*2*|**3**|`4`|~~5~~
___
<!-- CITA -->
## Cita
```
>Una cita es la idea que se extrae de un documento de manera textual o parafraseada que sirve de fundamento el trabajo.
>Este texto forma parte de la misma cita.
>>También se puede agregar dos mayores que y tomara una sangría dentro de la misma cita.

Corte de la cita anterior

>En el caso de esta cita podemos agregar comandos para destacar cierto texto **como esta sección este en negritas**, *también podemos agregar cursiva* o `agregar código en la misma cita` y ~~hasta tachar el texto~~.

```
>Una cita es la idea que se extrae de un documento de manera textual o parafraseada que sirve de fundamento el trabajo.
>Este texto forma parte de la misma cita.
>>También se puede agregar dos mayores que y tomara una sangría dentro de la misma cita.

Corte de la cita anterior

>En el caso de esta cita podemos agregar comandos para destacar cierto texto **como esta sección este en negritas**, *también podemos agregar cursiva* o `agregar código en la misma cita` y ~~hasta tachar el texto~~.

---
## Separador
```
Para realizar los separados es necesario
Tres o mas
---
Guiones medios,
***
Asteriscos,
___
Guiones bajos
___
```
Para realizar los separados es necesario

Tres o mas

---
Guiones medios
***
Asteriscos
___
Guiones bajos
___
<!-- LISTA DE TAREAS -->
```
* [x] Para realizar una lista de tareas comenzamos con un `asterisco` o `guio medio`
- [ ] Abrimos corchetes, en caso de que la tarea este finalizada
* [x] Ingresamos una `X` dentro de los corchetes como en este ejemplo
- [ ] En caso de que la tarea no esté finalizada, dejamos vacío los corchetes
* [x] En este ejemplo tiene un X dentro de los corchetes
```
* [x] Para realizar una lista de tareas comenzamos con un `asterisco` o `guio medio`
- [ ] Abrimos corchetes, en caso de que la tarea este finalizada
* [x] Ingresamos una `X` dentro de los corchetes como en este ejemplo
- [ ] En caso de que la tarea no esté finalizada, dejamos vacío los corchetes
* [x] En este ejemplo tiene un X dentro de los corchetes
---
<!-- EMOJI -->
Podemos agregar emojis a nuestro repositorio, para conocer los comandos en el siguiente enlace te muestra todos los comandos de los [emojis](https://gist.github.com/rxaviers/7360908) 
```
:frowning_face: 
:heart_eyes:
:grin:
```
:frowning_face: 

:heart_eyes:

:grin: