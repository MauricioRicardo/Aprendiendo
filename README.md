# Aprendiendo

En este lugar guardare los comandos con mi concepto sobre el

<!-- HEADINGS -->
# Comandos
## Titulo Tamaño #2
### Titulo Tamaño #3
#### Titulo Tamaño #4
##### Titulo Tamaño #5
---
<!-- ITALICA -->
*Este es un texto en Italica*
___
<!-- NEGRITAS -->
**Este es un texto en Negritas**
___
<!-- TACHADO -->
~~Este es un texto Tachado~~
___
<!-- LISTA DESORDENADA -->
Colores
* Rojo
    * Naranja
        * Rosa
* Azul
    * Verde
        * Negro
* Amarillo
    * Violeta
        * Blanco
---
<!-- LISTA ORDENADA -->
1. Rojo
    1. Naranja
1. Azul
    1. Verde
1. Amarillo
    1. Violeta
___
<!-- ENLASE -->
[Cuanto Falta Para Navidad](https://reloj-alarma.es/temporizador/navidad/ "Saber Cuanto Tiempo Falta Para Navidad")
___
<!-- CITA -->
> Esto es una Cita
---
<!-- ETIQUETAS DE CODIGO -->
`console.log(Hello Word)`
___
<!-- BLOQUE DE CODIGO -->
```js 
import axios from 'axios';
import { defineStore } from 'pinia';
import login from '../services/login.js';
export const useLoginStore = defineStore('login', {
    state: () => ({
        email: "",
        password: "",
        isUserBlocked: false,
        isDisabled: true,
        isLoading: false,
        isError: false,
        errorMessage: ""
    }),   
    }
});
```
---
<!-- TABLAS -->
|    Carro   |   Color   |    Modelo   |    Año    |
|------------|-----------|-------------|-----------|
| Celica     | Negro     | GTS         | 2006      |
| Honda      | Azul      | Civic       | 2001      |
|Tesla      |Blanco     |S            |2020       |
|Land Rover|Gris|Defender|2023
Lincoln|Dorado|Navigator|2020
---
<!-- IMAGENES -->
![Gomu Gomu No MI](https://res.cloudinary.com/dtzgksveo/image/upload/v1685749807/PitooPlumo/Gomu_Gomu_No_Mi_zdoelc.png "Gomu Gomu No Mi")
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