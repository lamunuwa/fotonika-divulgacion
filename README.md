# Fotonika, divulgación científica de óptica

Repositorio central para la coordinación, gestión y desarrollo de la plataforma web del proyecto de divulgación científica en óptica.

> **Nota:** La elaboración de experimentos y contenidos teóricos se realiza en herramientas externas o en vida real y se integra progresivamente en este repositorio.

---

## Propósito del Repositorio

- **Gestión del proyecto:** Centralizar el seguimiento de tareas y requerimientos a través del tablero de GitHub (Projects), Issues y Pull Requests supervisados por el Project Manager (@LaMunuwa).
- **Desarrollo Web:** Base para la creación y despliegue de la página web oficial del proyecto (ubicada en `/web`).
- **Almacenamiento Estructurado de Materiales:** Repositorio ordenado para foros de discusión, tablas de datos e imágenes generadas durante los experimentos.

---

## Estructura del Proyecto

```text
fotonika-divulgacion/
├── .github/                 # Plantillas de gestión (Issues, Pull Requests)
│   ├── ISSUE_TEMPLATE/      # Plantillas para bugs, mejoras y carga de contenido
│   └── PULL_REQUEST_TEMPLATE.md
├── docs/                    # Documentación y materiales de divulgación
│   ├── foros/               # Guías temáticas y foros (Refracción, Dispersión, Lentes)
│   ├── images/              # Recursos gráficos, fotografías y esquemas
│   └── tablas/              # Tablas de mediciones y resultados experimentales
├── web/                     # Código fuente de la plataforma web
├── compose.yml              # Configuración de servicios y contenedores
└── README.md                # Documentación principal del proyecto
```

---

## Flujo de Trabajo y Gestión

Para mantener el orden del proyecto:

1. **Commits:** todo commit subido debe llevar uso de conventional commits simple (sin optional scope). [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
2. **Issues:** toda tarea, reporte de error, propuesta web o subida de material experimental debe tener una Issue registrada usando las plantillas de `.github/ISSUE_TEMPLATE/`, usalas integrando un label `enhancement`, `bug` o `documentation`.
3. **Ramas (Branches):** trabajar en ramas temáticas según el tipo de cambio:
   - `feature/<nombre>` para desarrollo en `/web`.
   - `docs/<tema>` o `data/<tema>` para incorporación de materiales en `/docs`.
   - `fix/<descripcion>` para correcciónes.
4. **Pull Requests:** todo cambio se somete a revisión mediante Pull Request enlazado a su Issue correspondiente (`Closes #ID`) y debe cumplir con la lista de verificación establecida en la plantilla de PR.
