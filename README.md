# Sintaxis Markdown
Este espacio es para tener a la mano la sintaxis de los diferentes comandos con sus variables y sus diferentes formas de realizar la misma acción.

<!-- HEADINGS -->
# :diamond_shape_with_a_dot_inside: Encabezados
```
# Encabezado Tamaño 1
## Encabezado Tamaño 2
### Encabezado Tamaño 3
#### Encabezado Tamaño 4
##### Encabezado Tamaño 5

Una alternativa para los encabezados de tamaño 1 y 2 con subrayado es:

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

Una alternativa para los encabezados de tamaño 1 y 2 con subrayado es:

Alternativa Encabezado Tamaño 1
=
Alternativa Encabezado Tamaño 2
-
---
<!-- CURSIVA - NEGRITAS - TACHADO -->
# :diamond_shape_with_a_dot_inside: Estilos de Texto
```
Para darle el estilo con *Cursiva*, es con *asteriscos* o _guiones bajos_ 
Para darle el estilo con **Negrita**, es con dos **asterisco** o __guiones bajos__
Para darle el estilo combinado, es con **asteriscos y _guiones bajos_**
Para darle el estilo con <sub>subíndice</sub> es con la etiqueta <sub>sub</sub>
Para darle el estilo con <sup>superíndice</sup> es con la etiqueta <sup>sup</sup>
Para tachar el texto es con dos ~~virgulillas~~
```
Para darle el estilo con *Cursiva*, es con *asteriscos* o _guiones bajos_.

Para darle el estilo con **Negrita**, es con dos **asterisco** o dos __guiones bajos__.

Para darle el estilo combinado, es con **asteriscos y _guiones bajos_**.

Para darle el estilo con <sub>subíndice</sub> es con la etiqueta <sub>sub</sub>.

Para darle el estilo con <sup>superíndice</sup> es con la etiqueta <sup>sup</sup>.

Para tachar el texto es con dos ~~virgulillas~~.

<!-- LISTA DESORDENADA -->
# :diamond_shape_with_a_dot_inside: Lista Ordenada
```
1. Primer elemento de una lista ordena
2. Segundo elemento de una lista ordena
9. El valor del número no importa, solo debe ser un número
    1. Sub lista ordenado
    5. Sub lista con número que no es consecutivo del anterior
7. Otro elemento
    Para tener un párrafo de texto con sangría dentro de una lista, solo tenemos que presionar la tecla de tabulador `TAB`
```
1. Primer elemento de una lista ordena
2. Segundo elemento de una lista ordena
9. El valor del número no importa, solo debe ser un número
    1. Sub lista ordenado
    5. Sub lista con número que no es consecutivo del anterior
7. Otro elemento  
    Para tener un párrafo de texto con sangría dentro de una lista, solo tenemos que presionar la tecla de tabulador `TAB`.
___
<!-- LISTA ORDENADA -->
# :diamond_shape_with_a_dot_inside: Lista Desordenada
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
# :diamond_shape_with_a_dot_inside: Enlaces
Para realizar enlaces hay dos formas **Relativas** (dentro del proyecto) y **Absolutas** (fuera del proyecto):
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
# :diamond_shape_with_a_dot_inside: Imagenes
```
El logo de Pi (Al pasar el cursor sobre el logo mostrara un título)
Imagen en línea:
![Pi](https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")

Imagen referenciada de nuestro proyecto:
![PI](https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")

Imagen que cambia dependiendo el tema que tengamos en nuestro equipo en caso de que el tema sea oscuro se mostrar una luna en caso de que el tema sea claro se mostrara un sol

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/Luna_gzuafj.png">

  <source media="(prefers-color-scheme: light)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/sol_lxxaqy.png">
  
  <img alt="Esta imagen se mostrar en caso de que ninguna de las anterior se pueda mostrar" src="https://res.cloudinary.com/dtzgksveo/image/upload/v1686090395/PitooPlumo/Eclipse_c3zooy.png">
</picture>
```
El logo de Pi (Al pasar el cursor sobre el logo muestra un título)

Imagen en línea:
![Pi](https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")

Imagen referenciada de nuestro proyecto:
![PI](./Recursos/Pi.png "Logo de Pi")

Imagen que cambia dependiendo el tema que tengamos en nuestro equipo en caso de que el tema sea oscuro se mostrar una luna en caso de que el tema sea claro se mostrara un sol:

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/Luna_gzuafj.png">

  <source media="(prefers-color-scheme: light)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/sol_lxxaqy.png">
  
  <img alt="Esta imagen se mostrar en caso de que ninguna de las anterior se pueda mostrar" src="https://res.cloudinary.com/dtzgksveo/image/upload/v1686090395/PitooPlumo/Eclipse_c3zooy.png">
</picture>

___
<!-- BLOQUE DE CODIGO -->
# :diamond_shape_with_a_dot_inside: Código 
Los bloques de código forman parte de la especificación de Markdown, pero el resaltado de sintaxis no. Sin embargo, muchos renderizados como GitHub lo soportan.

```
El `código` que quieras resaltar como código al su alrededor tiene `acento grave`.
```
El `código` que quieras resaltar al su alrededor tiene `acentos graves`.

Los bloques de código están  delimitados por **tres acentos graves** ` ``` `:

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
# :diamond_shape_with_a_dot_inside: Etiquetas HTML
También se puede utilizar etiquetas HTML sin formato y la mayoría de ellas funcionan en GitHub.
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
# :diamond_shape_with_a_dot_inside: Sección Desplegable
Para realizar la sección desplegable es necesario usar la etiqueta `<details>`

```html
<details>
<summary>El titulo de la sección desplegable </summary>
    Hola mundo
</details>
```
<details>
<summary>El titulo de la sección desplegable </summary>
    Hola mundo
</details>

---

# :diamond_shape_with_a_dot_inside: Nota a Pie de Página
Las notas a pie no forman parte de la especificación de Markdown, pero son soportadas por GitHub.
```
Esto es unas nota a pie simples[^1]

Una nota a pie también puede tener varias líneas[^2]

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

[^2]: Cada nueva línea debe ir antes dos espacios.
  Esto permite tener una nota con varias líneas.

 [^nota]:
    Las notas con nombre seguirán mostrando números en lugar de texto, pero permiten una mejor identificación y un enlace más sencillo.

    Esta nota también se ha hecho con una sintaxis diferente utilizando cuatro espacios para las nuevas líneas.
___
<!-- TABLAS -->
# :diamond_shape_with_a_dot_inside: Tabla
Las tablas no forman parte de las especificaciones de Markdown, pero GitHub las soporta.
```
Se puede utilizar **dos puntos** `:` para alinear las columnas:

|    Carro   |  Color  |   Modelo  |  Año  |
|------------|:-------:|----------:|-------|
| Celica     | Negro   | GTS       | 2006  |
| Honda      | Azul    | Civic     | 2001  |
| Tesla      | Blanco  | S         | 2020  |
| Land Rover | Gris    | Defender  | 2023  |
| Lincoln    | Dorado  | Navigator | 2020  |

Las plecas `|` del exterior son opcionales, no es necesario para realizar la tabla igual que la alineación no es necesaria.

Debe haber al menos **tres guiones medios** para realizar la cabecera.

Dentro de las columnas también se pueden utilizar los comandos para darle estilo a cierto texto:

Normal|Cursiva|Negrita|Código|Tachado
:---:|:---:|:---:|:---:|:---:|
Markdown|*Markdown*|**Markdown**|`Markdown`|~~Markdown~~
1|*2*|**3**|`4`|~~5~~
```
Se puede utilizar **dos puntos** `:` para alinear las columnas:

|    Carro   |  Color  |   Modelo  |  Año  |
|------------|:-------:|----------:|-------|
| Celica     | Negro   | GTS       | 2006  |
| Honda      | Azul    | Civic     | 2001  |
| Tesla      | Blanco  | S         | 2020  |
| Land Rover | Gris    | Defender  | 2023  |
| Lincoln    | Dorado  | Navigator | 2020  |

Las **plecas** `|` del exterior son opcionales, no es necesario para realizar la tabla igual que la alineación no es necesaria.

Debe haber al menos **tres guiones medios** para realizar la cabecera.

Dentro de las columnas también se pueden utilizar los comandos para darle estilo a cierto texto:

Normal|Cursiva|Negrita|Código|Tachado
:---:|:---:|:---:|:---:|:---:|
Markdown|*Markdown*|**Markdown**|`Markdown`|~~Markdown~~
1|*2*|**3**|`4`|~~5~~
___
<!-- CITA -->
# :diamond_shape_with_a_dot_inside: Cita
```
>Una cita es la idea que se extrae de un documento de manera textual o parafraseada que sirve de fundamento el trabajo.
>Este texto forma parte de la misma cita.
>>También se puede agregar **dos mayores que** `>` y tomara una sangría dentro de la misma cita.

Corte de la cita anterior.

>En el caso de esta cita podemos agregar comandos para destacar cierto texto **como esta sección este en negritas**, *también podemos agregar cursiva* o `agregar código en la misma cita` y ~~hasta tachar el texto~~.

```
>Una cita es la idea que se extrae de un documento de manera textual o parafraseada que sirve de fundamento el trabajo.
>Este texto forma parte de la misma cita.
>>También se puede agregar **dos mayores que** `>` y tomara una sangría dentro de la misma cita.

Corte de la cita anterior.

>En el caso de esta cita podemos agregar comandos para destacar cierto texto **como esta sección este en negritas**, *también podemos agregar cursiva* o `agregar código en la misma cita` y ~~hasta tachar el texto~~.

---
# :diamond_shape_with_a_dot_inside: Separador
```
Para realizar los separados es necesario:
Tres o mas
---
Guiones medios `-`
***
Asteriscos `*`
___
Guiones bajos `_`
___
```
Para realizar los separados es necesario:

Tres o mas

---
Guiones medios `-`
***
Asteriscos `*`
___
Guiones bajos `_`
___
<!-- LISTA DE TAREAS -->
# :diamond_shape_with_a_dot_inside: Lista de Tareas
```
* [x] Para realizar una lista de tareas comenzamos con un **asterisco** `*` o **guion medio** `-`
- [ ] Abrimos **corchetes** `[]`, en caso de que la tarea esté finalizada
* [x] Ingresamos una `X` dentro de los corchetes como en esté ejemplo
- [ ] En caso de que la tarea no esté finalizada, dejamos vacío los corchetes
* [x] En este ejemplo tiene un `X` dentro de los corchetes.
```
* [x] Para realizar una lista de tareas comenzamos con un **asterisco** `*` o **guion medio** `-`
- [ ] Abrimos **corchetes** `[]`, en caso de que la tarea esté finalizada
* [x] Ingresamos una `X` dentro de los corchetes como en esté ejemplo
- [ ] En caso de que la tarea no esté finalizada, dejamos vacío los corchetes
* [x] En este ejemplo tiene un `X` dentro de los corchetes.
___

<!-- EMOJI -->
# :diamond_shape_with_a_dot_inside: Emoji
Podemos agregar emojis a nuestro repositorio, para conocer los comandos en el siguiente enlace te muestra todos los códigos de los [emojis](https://github-emoji-picker.rickstaa.dev/)
```
:frowning_face: - :heart_eyes: - :grin:

<details>
<summary>Lista de Emoji </summary>

Emoji|Emoji|Emoji
:---:|:---:|:---:
:diamond_shape_with_a_dot_inside: `:diamond_shape_with_a_dot_inside:` | :fast_forward: `:fast_forward:` | :arrow_forward: `:arrow_forward:`
:sparkles: `:sparkles:` | :point_right: `:point_right:` | :cyclone: `:cyclone:`
:milky_way: `:milky_way:` | :sparkler: `:sparkler:` | :space_invader: `:space_invader:`
:triangular_flag_on_post: `:triangular_flag_on_post:` | :eight_spoked_asterisk: `:eight_spoked_asterisk:` |  :alien: `:alien:`
:eight_pointed_black_star: `:eight_pointed_black_star:` | :white_check_mark: `:white_check_mark:` | :red_circle: `:red_circle:`
:pirate_flag: `:pirate_flag:` | :gear: `:gear:` | :robot: `:robot:`
:speech_balloon: `:speech_balloon:` |  :fire: ` :fire:` | :collision: `:collision:`

</details>
```
:frowning_face: - :heart_eyes: - :grin:

<details>
<summary>Lista de Emoji </summary>

Emoji|Emoji|Emoji
:---:|:---:|:---:
:diamond_shape_with_a_dot_inside: `:diamond_shape_with_a_dot_inside:` | :fast_forward: `:fast_forward:` | :arrow_forward: `:arrow_forward:`
:sparkles: `:sparkles:` | :point_right: `:point_right:` | :cyclone: `:cyclone:`
:milky_way: `:milky_way:` | :sparkler: `:sparkler:` | :space_invader: `:space_invader:`
:triangular_flag_on_post: `:triangular_flag_on_post:` | :eight_spoked_asterisk: `:eight_spoked_asterisk:` |  :alien: `:alien:`
:eight_pointed_black_star: `:eight_pointed_black_star:` | :white_check_mark: `:white_check_mark:` | :red_circle: `:red_circle:`
:pirate_flag: `:pirate_flag:` | :gear: `:gear:` | :robot: `:robot:`
:speech_balloon: `:speech_balloon:` |  :fire: ` :fire:` | :collision: `:collision:`

</details>

---