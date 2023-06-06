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

Una alternativa para los encabezados de tamaño 1 y 2 con subrayado es:

Alternativa de Encabezado 1
=
Alternativa de Encabezado 2
-
---
<!-- CURSIVA - NEGRITAS - TACHADO -->
## Estilos de Texto
```
Para indicar énfasis con *Cursiva*, es con *astericos* o _guiones bajos_ 
Para indicar énfasis con **Negrita**, es con dos **asterisco** o __guiones bajos__
Para indicar énfasis combinado, es con **asteriscos y _guioenes bajos_**
Para indicar enfasis con <sub>subindice</sub> es con la etiqueta <sub>sub</sub>
Para indicar enfasis con <sup>superindice</sup> es con la etiqueta <sup>sup</sup>
Para tachar el texto. es con dos ~~virgulillas~~
```
Para indicar énfasis con *Cursiva*, es con *astericos* o _guiones bajos_ 

Para indicar énfasis con **Negrita**, es con dos **asterisco** o __guiones bajos__

Para indicar énfasis combinado, es con **asteriscos y _guioenes bajos_**

Para indicar enfasis con <sub>subindice</sub> es con la etiqueta <sub>sub</sub>

Para indicar enfasis con <sup>superindice</sup> es con la etiqueta <sup>sup</sup>

Para tachar el texto. es con dos ~~virgulillas~~
___
<!-- LISTA DESORDENADA -->
## Lista Ordenada
```
1. Primer elemento de una lista ordena
2. Segundo elemento de una lista ordena
9. El valor del numero no impora, con que solo sea un numero
    1. Sub lista ordenado
    5. Sub lista con numero que no consecutivo del anterior
7. Otro elemento
```
1. Primer elemento de una lista ordena
2. Segundo elemento de una lista ordena
9. El valor del numero no impora, con que solo se un numero
    1. Sub lista ordenado
    5. Sub lista con numero que no consecutivo del anterior
7. Otro elemento

    Para tener un parrafo de texto con sangria dentro de una lista, solo tenemos que precionar la tecla de tabulador (TAB)
___
<!-- LISTA ORDENADA -->
## Lista Desordenada
```
* Las lista desordenada puedes usar asterisco
    * Sub lista desordena
        * Sub lista de la sub lista anterior
- Tambien puedes utilizar un menos
    + Tambien puedes utilizar el mas
        * O combinar las tres formas anteriores
```
* Las lista desordenada puedes usar asterisco
    * Sub lista desordena con asterisco
        * Sub lista de la sub lista anterior con asterisco
- Tambien puedes utilizar un menos
    + Tambien puedes utilizar el mas
        * O combinar las tres formas anteriores
___
<!-- ENLASE -->
## Enlaces
Para realizar enlaces hay dos formas relativas(Dentro del proyecto) y absolutas(Fuera del proyecto)
```
[Enlace absoluto en linea](https://www.youtube.com/)

[Enlace absoluto en linea](https://www.youtube.com/ "Pagina principal de YouTube")

[Enlace absoluto con referencia][El texto de referencia deve ser insensitive para no tener problemas con el enlace]

[Tambien se puede utilizar números para definir el enlace absoluto de referencia][1]

o podemos dejar vacio y utilizar el [texto del enlace]

[Enlace relativo con referencia a un archivo del repositorio](./Luffy.md)

[El texto de referencia deve ser insensitive para no tener problemas con el enlace]: https://www.mozilla.org
[1]: /www.google.com
[texto del enlace]: http://www.reddit.com 
```

[Enlace absoluto en linea](https://www.youtube.com/)

[Enlace absoluto en linea con titulo](https://www.youtube.com/ "Pagina principal de YouTube")

[Enlace absoluto con referencia][El texto de referencia deve ser insensitive para no tener problemas con el enlace]

[Enlace relativo con referencia a un archivo del repositorio](./Recursos/Luffy.md)

[Tambien se puede utilizar números para definir el enlace absoluto de referencia][1]

o podemos dejar vacio y utilizar el [texto del enlace]

[El texto de referencia deve ser insensitive para no tener problemas con el enlace]: https://www.mozilla.org
[1]: https://www.google.com
[texto del enlace]: http://www.reddit.com 
___
<!-- IMAGENES -->
## Imagenes
```
El logo de Pi (Al pasar el cursor sobre el logo mostrara un titulo)
Imagen en linea:
![Pi]
(https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")

Imegen referenciada de nuestro proyecto:
![PI](https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")
```
El logo de Pi (Al pasar el cursor sobre el logo muestra un titulo)

Imagen en linea:
![Pi](https://res.cloudinary.com/dtzgksveo/image/upload/v1685985500/PitooPlumo/Pi_zec9ef.png "Logo de Pi")

Imegen referenciada de nuestro proyecto:
![PI](./Recursos/Pi.png "Logo de Pi")

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/Luna_gzuafj.png">

  <source media="(prefers-color-scheme: light)" srcset="https://res.cloudinary.com/dtzgksveo/image/upload/v1686083035/PitooPlumo/sol_lxxaqy.png">
  
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>

___
<!-- BLOQUE DE CODIGO -->
## Codigo 
Los bloques de código forman parte de la especificación de Markdown, pero el resaltado de sintaxis no. Sin embargo, muchos renderiadores, como GitHub y Markdown Here, soportan el resaltado de sintaxis. Que lenguajes son soportados y cómo deben escribirse los nombres de eos lenguajes varia de un rendirezador a otro.

```
El `codigo` que quieras resaltar como codigo al su alrededor tiene acento `grave`
```
El `codigo` que quieras resaltar al su alrededor tiene `acento grave`

Los bloques de codigo estan delimitados por tres acentos graves ` ``` `

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
## Nota a Pie de Página
Las notas no forman parte de la especificaicon de Markdown, pero son soportadas por GitHub
```
Esto es unas notas simples[^1]

Una nota tambien puede tener varias lineas[^2]

Tambien se puede utilizar palabras, para la referencia[^nota]

[^1]: Mi referencia

[^2]: Cada nueva linea debe ir antes dos espacios
 Esto permite tener una nota con varias linesas
 [^nota]:
    Las not con nombre seguiran mostando numeros en lugar de texto, pero permiten una identificacion y un enlace mas sencullo.
    Esta nota tambien se ha hecho con una sintaxis diferente utilizando cuatro espacio para las nuevas lineas.
```
Esto es unas notas simples[^1]

Una nota tambien puede tener varias lineas[^2]

Tambien se puede utilizar palabras, para la referencia[^nota]

[^1]: Mis referencia

[^2]: Cada nueva linea debe ir antes dos espacios
 Esto permite tener una nota con varias linesas
 [^nota]:
    Las not con nombre seguiran mostando numeros en lugar de texto, pero permiten una identificacion y un enlace mas sencullo.
    Esta nota tambien se ha hecho con una sintaxis diferente utilizando cuatro espacio para las nuevas lineas.
___
<!-- TABLAS -->
## Tabla
Las tablas no forman parte de las especificaciones de Markdown, pero GitHub las soporta
```
Se puede utilizr dos puntos para alinear las columnas

|    Carro   |  Color  |   Modelo  |  Año  |
|------------|:-------:|----------:|-------|
| Celica     | Negro   | GTS       | 2006  |
| Honda      | Azul    | Civic     | 2001  |
| Tesla      | Blanco  | S         | 2020  |
| Land Rover | Gris    | Defender  | 2023  |
| Lincoln    | Dorado  | Navigator | 2020  |

Debe haber al menos tres guiones para realizar la cabezara.
Las plecas (|) del exterior son opcionales y no es necesario para realizar la tabla igual que la alineacio no es necesaria. Dentro de las columnas tambien se pueden utilizar los destacar

Normal|Cursiba|Negrita|Codigo
---|---|---|---|
Markdown|*Markdown*|**Markdown**|`Markdown`|
1|2|3|4
```
Se puede utilizr dos puntos para alinear las columnas

|    Carro   |  Color  |   Modelo  |  Año  |
|------------|:-------:|----------:|-------|
| Celica     | Negro   | GTS       | 2006  |
| Honda      | Azul    | Civic     | 2001  |
| Tesla      | Blanco  | S         | 2020  |
| Land Rover | Gris    | Defender  | 2023  |
| Lincoln    | Dorado  | Navigator | 2020  |

Debe haber al menos tres guiones para realizar la cabezara.
Las plecas (|) del exterior son opcionales y no es necesario para realizar la tabla igual que la alineacio no es necesaria. Dentro de las columnas tambien se pueden utilizar los comandos para destarcar cierto texto

Normal|Cursiba|Negrita|Codigo|Tachado
---|---|---|---|---|
Markdown|*Markdown*|**Markdown**|`Markdown`|~~Markdown~~
1|*2*|**3**|`4`|~~5~~
___
<!-- CITA -->
## Cita
```
>Una cita es la idea que se extrae de un documento de manera textual o parafraseada que sirve de fundamento el trabajo.
>Este texto forma parte de la misma cita.

Corte de la cita anterior

>En el caso de esta cita podemos agregar comandos para destacar cierto texto **como esta seccion este en negritas**, *tambien podemos agregar cursiva* o `gregar codigo en la misma cita` y ~~hasta tachar el texto~~.
```
>Una cita es la idea que se extrae de un documento de manera textual o parafraseada que sirve de fundamento el trabajo.
>Este texto forma parte de la misma cita.
>>Tambien se puede agregar dos mayor que y tomara una sangria dentro de la misma cita.

Corte de la cita anterior

>En el caso de esta cita podemos agregar comandos para destacar cierto texto **como esta seccion este en negritas**, *tambien podemos agregar cursiva* o `gregar codigo en la misma cita` y ~~hasta tachar el texto~~.

---
## Codigo HTML
Tambien se puede utilizar codigo HTML sin formarmato y la mayoria de las funciones se pueden utilizar
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

## Separador
```
Con tres o mas
---
Guiones medios
***
Asteriscos
___
Guiones bajos
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
<!-- GITHUB MARKDOWN -->
* [x] Tarea 1
* [ ] Tarea 2
* [x] Tarea 3
* [ ] Tarea 4
* [x] Tarea 5
---
<!-- EMOJI -->
:frowning_face: 
:heart_eyes:
:grin:
___
