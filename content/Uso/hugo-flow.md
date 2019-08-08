
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
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media 

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

