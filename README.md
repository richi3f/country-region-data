## country-region-data 

*Traducción del repositorio de [benkeen](https://github.com/benkeen)*

Este repositorio contiene un archivo JSON estático compuesto por países, sus códigos ISO 3166-2 y sus estados/provincias también con sus códigos ISO 3166-2.

Este repositorio fue creado por [benkeen](https://github.com/benkeen) para albergar la información fuente de sus scripts: [country-region-selector](https://github.com/benkeen/country-region-selector) y
[react-country-region-selector](https://github.com/benkeen/react-country-region-selector).

Véase el archivo `data.json` para obtener los datos. El JSON se encuentra de la siguiente forma:

```javascript
[
  {
    "countryName":"Ecuador",
    "countryShortCode":"EC",
    "regions":[
      {
        "name":"Azuay",
        "shortCode":"A"
      },
      ...
    }
  },
  ... 
]
```

### Contribuye

Las abreviaciones de los estados/provincias aún no están completas, ¡por lo que las contribuciones son bienvenidas! Cada estado/provinica que carece de un código ISO 3166-2 puede ser identificado a través de su propiedad `shortCode`. Clona este repositorio y ejecuta:

```
npm install
grunt findIncomplete
```

Esto enlistará todo país con regiones incompletas. La información faltante se puede encontrar en Wikipedia:
https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2


### Valida

Antes de contribuir, valida el contenido JSON. Para esto ejecuta lo siguiente en tu línea de comando:

```
npm install
grunt validate
```

Esto lanzará un error si el JSON es inválido o si existen nombres duplicados que fueron accidentalmente insertados. Los mensajes de error deberían ser muy claros.


### Cambios

- `1.3.7` - 2 de enero de 2017. Traducción del inglés a todos los países y regiones hispanohablantes
- `1.0.0` - 29 de abril de 2016. Version inicial de [benkeen](https://github.com/benkeen)


### Licencia

MIT.
