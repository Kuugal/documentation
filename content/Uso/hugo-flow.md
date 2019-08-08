
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

- [ ] Push de la branch Dev local a origin
- [ ] Checkout a rama Deploy, merge desde Dev
- [ ] Modificar el *config.toml* en *baseURL = "https://kuugal.github.io/documentation/"*
- [ ] Compilar a modo producción con `hugo -d public` estando en la carpeta del proyecto
- [ ] Push de la rama local a origin
- [ ] Merge desde Deploy a origin/gh-pages


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

