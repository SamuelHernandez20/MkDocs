# Creación de un sitio web estático | MkDocs
**MkDocs** es un generador de sitios web estáticos que nos permite crear de forma sencilla un sitio web para documentar un proyecto. 
El contenido del sitio web está escrito en texto plano en formato Markdown y se configura con un único archivo de configuración en formato **YAML**.

La estructura de directorios que sigo para esta práctica es así:

``
.
├── .github
└── workflows
│   │   └── build-push-mkdocs.yaml
└── proyecto
    ├── docs
    │   └── index.md
    └── mkdocs.yml
``