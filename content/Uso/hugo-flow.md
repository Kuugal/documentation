
---
title: "Hugo"
tags: ["hugo", "CMS"]
menuTitle : "Hugo flow"
---
### Nuevo documento
___
1. Crea un archivo con extensión markdown **.md** en el directorio pertinente

2. Agrega el header _YAML o TOML_ al archivo
```
---
title: "Hugo"
tags: ["hugo", "CMS"]
menuTitle : "Hugo flow"
---
```

2. Se agrega el logo (720px) **Sólo si es md de instalación** 
```
<img src="/img/hugo-logo.svg" width="720">
```
3. Agrega contenido de manera organizada
```
### Nuevo documento
___
1. Crea un archivo con extensión markdown **.md** en el directorio pertinente
```

### Deploy
___

1. Push de la branch Dev local a origin
2. Eliminar rama gh-pages
3. Crear rama gh-pages desde Dev y checkout
4. Modificar el *config.toml* en `baseURL = "https://kuugal.github.io/documentation/"`
5. Compilar a modo producción con `hugo -d public` estando en la carpeta del proyecto
6. Push de la rama local a origin


{{% notice note %}}
Los cambios en el servidor tardarán un minuto en verse reflejados
{{% /notice %}}

### Configuración
___

#### Rutas

* **Favicon**
/themes/learn/layouts/partials/favicon.html
* **Logo**
/themes/learn/layouts/partials/logo.html
* **Imagenes**
/themes/learn/static/images/ _(.png or .ico)_
* **Variante del tema**
/config.toml
```
[params]
  # Change default color scheme with a variant one. Can be "red", "blue", "green".
  themeVariant = "red"

```

