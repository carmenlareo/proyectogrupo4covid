# 🦠 COVID-19 Tracker — Dashboard de Gestión de Pandemias

Bienvenida al equipo de desarrollo! 👋 Este README explica cómo trabajar en el repositorio y cómo gestionar las tareas del proyecto usando GitHub Projects. Léelo con calma antes de empezar.

---

## 🎮 Contexto del proyecto

Nuestra consultora nos ha contratado para desarrollar el front-end de un **Dashboard de Gestión de Datos de Pandemias**, enfocado en el **COVID-19**. El proyecto se desarrolla con **React + Vite**, consumiendo datos de la API de [disease.sh](https://disease.sh/).

### Objetivos

- Proporcionar una plataforma interactiva de visualización de datos
- Análisis de datos en tiempo real
- Escalabilidad para futuras pandemias

---

## 🛠️ Tecnologías

| Tecnología | Para qué la usamos |
| ----------- | ------------------------------------------------ |
| **React** | Librería para construir la interfaz por componentes |
| **Vite** | Herramienta de desarrollo y bundling |
| **React Router** | Navegación entre las páginas del dashboard |
| **Axios** | Consumo de la API de disease.sh |
| **Sass + CSS Modules** | Estilos con alcance local por componente |
| **Git + GitHub** | Control de versiones y trabajo en equipo |

---

## 💻 Instalación en local

### Requisitos previos

- [Node.js](https://nodejs.org/) (v18 o superior)
- [Git](https://git-scm.com/)
- [VS Code](https://code.visualstudio.com/) (recomendado)

### Pasos para instalar

```bash
# 1. Clona el repositorio
git clone https://github.com/TU-USUARIO/covid-tracker.git

# 2. Entra en la carpeta del proyecto
cd covid-tracker

# 3. Instala las dependencias
npm install

# 4. Arranca el servidor de desarrollo
npm run dev
```

> 💡 Se abrirá en `http://localhost:5173`. Cada vez que guardes un archivo, los cambios se ven automáticamente en el navegador.

---

## 📁 Estructura de carpetas

```
covid-tracker/
├── public/                  # Archivos estáticos
├── src/
│   ├── assets/              # Imágenes, iconos, fuentes
│   ├── components/          # Componentes reutilizables
│   │   ├── Sidebar/         # Tracker 0 — barra lateral con datos globales
│   │   ├── Navbar/          # Barra de navegación superior
│   │   ├── StatCard/        # Tarjeta de estadísticas
│   │   ├── CountryTabs/     # Pestañas de selección de país
│   │   └── Layout/          # Estructura principal (Sidebar + contenido)
│   ├── pages/               # Páginas del dashboard (una por compañera)
│   │   ├── Tracker1/        # Dashboard por país con stat cards
│   │   ├── Tracker2/        # Tabla con paginación, búsqueda y ordenación
│   │   ├── Tracker3/        # Vista de datos adicional
│   │   └── Tracker4/        # Vista con filtro por países
│   ├── services/            # Servicio único de consumo de API
│   │   └── api.js           # TODAS las peticiones a disease.sh van aquí
│   ├── styles/              # Estilos globales y variables Sass
│   │   └── _variables.scss  # Colores, tipografías, breakpoints
│   ├── App.jsx              # Componente principal con las rutas
│   └── main.jsx             # Punto de entrada de React
├── .gitignore
├── package.json
├── vite.config.js
└── README.md
```

> ⚠️ **Regla del proyecto:** Solo debe existir UN único archivo de servicio de API (`services/api.js`). Todos los componentes piden datos a través de este archivo.

---

## 🌿 ¿Cómo está organizado el repositorio?

| Rama | Para qué sirve |
| ----------- | ------------------------------------------------------------- |
| `main` | Código final en producción. **Nadie sube aquí directamente.** |
| `develop` | Rama de integración. **Tampoco se sube directamente.** |
| `tu-rama` | Tu rama personal según la tarea. **Aquí es donde tú trabajas.** |
... (336 líneas restantes)