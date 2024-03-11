# Creación de un sitio web estático | MkDocs
**MkDocs** es un generador de sitios web estáticos que nos permite crear de forma sencilla un sitio web para documentar un proyecto. 
El contenido del sitio web está escrito en texto plano en formato Markdown y se configura con un único archivo de configuración en formato **YAML**.

La estructura de directorios que sigo para esta práctica es así:

 # Estructura de Directorios:

````
.
└── -github/workflows
└──docs
    │   ├── images
    │   ├── LAMP_RHEL.md
    │   └── LAMP_UBUNTU.md
└── mkdocs.yml

``````
## 1. Crear un nuevo proyecto (Comando: new)

En caso de empezar por esta primera parte en la creación de un nuevo proyecto, deberemos de situarnos sobre el directorio desde donde lo queremos crear, y a continuación lanzar el siguiente comando, haciendo uso de ``new``:

```
docker run --rm -it -p 8000:8000 -v "$PWD":/docs squidfunk/mkdocs-material new .
```

Una vez realizada la creación de este nuevo proyecto, en el directorio de este, podemos realizar la creación de nuestro archivo **YAML**, para así poder crear la estructura básica que tendrá el sitio tras ser publicado:

```
site_name: Samuel_mkdocs

nav:
    - Practica LAMP en RHEL: LAMP_RHEL.md
    - Practica LAMP en UBUNTU: LAMP_UBUNTU.md

theme: 
  name: material
  palette:
    primary: purple
    accent: pink
  logo: images/S.png
  font: 
   text: Fredoka
   code: Fredoka
```
