﻿# Feedback_4_Informatica_II
# Monorepo – Proyecto de Blog con Spring Boot, BFF Next.js y Frontend Vite + React

Este repositorio agrupa tres subproyectos:
1. **back**: API REST en Spring Boot para gestionar Posts.
2. **bff**: Back-for-Front en Next.js que hace proxy a la API de Spring.
3. **front-vite**: Cliente React + Vite + Tailwind que consume el BFF.

---

## Clonar con submódulos

Para trabajar con los tres proyectos debes clonar el repositorio incluyendo sus submódulos:

```bash
git clone --recurse-submodules
```

## Estructura de carpetas

```
/
├── back/         # API Spring Boot
├── bff/          # Next.js BFF proxy
└── front-vite/   # React + Vite + Tailwind
```

Cada subcarpeta incluye su propio \`README.md\` con instrucciones detalladas de instalación y ejecución.


## Flujo de trabajo

- Modifica el **backend** y prueba en \`http://localhost:8080/api/posts\`.
- El **BFF** recoge cambios y los expone en \`http://localhost:3000/api/posts\`.
- El **cliente Vite** consume el BFF y muestra datos en la UI.
