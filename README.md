# 🏗️ Constructinini

## 📖 Descripción del Proyecto

**Constructinini** es una aplicación web enfocada en la **gestión integral de proyectos de construcción**, permitiendo la coordinación eficiente entre **administradores, gerentes de proyecto y trabajadores**.

Su objetivo principal es **centralizar las operaciones en obra**, como el control de tareas, asistencia, recursos y comunicación interna, optimizando los flujos de trabajo y la trazabilidad de cada proyecto.

---

## 🚀 Características Principales

- 🔐 **Autenticación y roles** (Administrador, Project Manager, Trabajador)  
- 🏗️ **Gestión de proyectos** con estado, ubicación y descripción  
- ✅ **Gestión de tareas**: creación, asignación, seguimiento y comentarios  
- 📸 **Control de asistencia** con registro de fotos y ubicación  
- 🧱 **Gestión de recursos**: solicitudes y aprobaciones de materiales  
- 💬 **Sistema de comentarios** y carga de fotos en tareas  
- ☁️ **Integración completa con Supabase** (base de datos, autenticación y almacenamiento)

---

## 🧩 Tecnologías Utilizadas

| Tecnología | Descripción |
|-------------|-------------|
| **Vite + React** | Framework y entorno de desarrollo frontend |
| **Supabase** | Backend, base de datos y autenticación |
| **PostgreSQL** | Base de datos relacional (gestionada por Supabase) |
| **Tailwind CSS** | Framework de estilos |
| **JavaScript / JSX** | Lenguaje principal de desarrollo |

---

## ⚙️ Requisitos

- **Node.js** versión 18 o superior  
- **npm** versión 9 o superior (incluido con Node.js)  
- **Conexión a Internet** (para usar Supabase como backend)

---

## 🛠️ Instalación

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/usuario/Constructinini.git
   cd Constructinini
   ```

2. **Instalar dependencias**
   ```bash
   npm install
   ```

3. **Ejecutar en modo desarrollo**
   ```bash
   npm run dev
   ```

   La aplicación se abrirá en:  
   👉 [http://localhost:5173](http://localhost:5173)

---

## 📦 Scripts Disponibles

| Comando | Descripción |
|----------|--------------|
| `npm run dev` | Inicia el entorno de desarrollo |
| `npm run build` | Compila la aplicación para producción |
| `npm run preview` | Permite previsualizar la versión compilada localmente |

---

## 🧱 Estructura del Proyecto

```
Constructinini/
├── src/
│   ├── components/        # Componentes reutilizables
│   ├── pages/             # Vistas principales
│   ├── lib/
│   │   └── supabaseClient.js   # Configuración de conexión con Supabase
│   └── styles/            # Archivos de estilos
├── public/                # Recursos estáticos
├── package.json           # Dependencias y scripts
└── vite.config.js         # Configuración del entorno
```

---

## 👥 Roles de Usuario

| Rol | Descripción |
|------|--------------|
| **Administrador** | Gestiona usuarios, proyectos y recursos globales |
| **Project Manager** | Crea y supervisa proyectos, tareas y trabajadores asignados |
| **Trabajador** | Marca asistencia, consulta tareas y sube fotos de progreso |

---

## 💾 Base de Datos y Backend

El sistema utiliza **Supabase** como backend y base de datos, por lo que **no se requiere instalación local**.

Para conectar tu propio proyecto de Supabase, reemplaza las credenciales en:

```js
// src/lib/supabaseClient.js
const supabaseUrl = 'TU_PROJECT_URL';
const supabaseAnonKey = 'TU_ANON_KEY';
```

Supabase maneja:
- Autenticación de usuarios
- Base de datos PostgreSQL
- Almacenamiento de fotos (buckets `tasks_photos` y `attendance_photos`)

---

## 👨‍💻 Equipo de Desarrollo

| Nombre | Rol |
|--------|------|
| **Tomás Mejía García** | Backend Developer |
| Equipo colaborador | Frontend y base de datos |

---

## 📄 Licencia

Este proyecto fue desarrollado con fines **académicos** y está licenciado bajo la **MIT License**.

---

## 🧠 Notas

- Durante desarrollo:  
  Ejecuta `npm run dev` para trabajar en la aplicación.

- Antes de desplegar:  
  1. Ejecuta `npm run build` para crear la versión optimizada.  
  2. Usa `npm run preview` para probar la versión final localmente.  
  3. Sube la carpeta `dist` al servidor o servicio de hosting deseado.

---
