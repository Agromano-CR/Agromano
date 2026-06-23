# agricultural-management-system

Sistema de Gestión Agrícola moderno y escalable para la administración del personal en fincas agroindustriales, integrando Express y Prisma en el backend y React en el frontend, utilizando TypeScript de extremo a extremo.

## Descripción General

Agricultural Management System es una plataforma full-stack orientada a optimizar la gestión del recurso humano en operaciones agrícolas. Permite registrar y monitorear la asistencia del personal, planificar turnos y asignar tareas según la temporada y la demanda de trabajo.

El sistema automatiza el cálculo de pagos basados en horas laboradas o productividad, además de generar reportes de eficiencia laboral y costos operativos. También ofrece exportación de información en formatos PDF y Excel para facilitar la administración y el análisis de datos.

El proyecto está diseñado aplicando principios de Clean Architecture tanto en el backend como en el frontend, garantizando una solución mantenible, escalable y preparada para entornos reales.

Incluye:

- Registro y seguimiento de asistencia
- Gestión de trabajadores
- Planificación de turnos y asignación de tareas
- Cálculo automático de pagos por horas y productividad
- Seguimiento del rendimiento laboral
- Reportes de eficiencia y costos operativos
- Exportación de información a PDF y Excel
- Backend REST API con Express y Prisma
- Frontend moderno con React
- Arquitectura limpia y modular

## Características Principales

- Control de asistencia de trabajadores
- Gestión de tareas y turnos según temporadas agrícolas
- Cálculo automático de pagos
- Seguimiento de productividad y rendimiento
- Generación de reportes operativos
- Exportación de datos en PDF y Excel
- API REST modular con Express
- Persistencia con Prisma ORM
- Frontend con React y TypeScript
- Arquitectura limpia y desacoplada
- Código mantenible y escalable

## Tecnologías Utilizadas

### Backend (Express)

- Node.js
- TypeScript
- Express
- Prisma ORM
- PostgreSQL
- Clean Architecture
- Repository Pattern
- DTOs
- Validaciones
- Arquitectura modular

### Frontend (React)

- React
- TypeScript
- React Router
- Componentes reutilizables
- Manejo de estado
- Formularios con validación
- Clean Architecture

### Exportación de Datos

- PDF
- Excel (.xlsx)

### Tooling

- NPM
- Git & GitHub
- ESLint
- Prettier

## Arquitectura del Proyecto

El proyecto está dividido en dos grandes módulos:

### Backend (Express + Prisma)

```bash
/src
├── domain                 # Entidades y contratos
├── application            # Casos de uso
├── infrastructure
│   ├── database
│   ├── repositories
│   ├── prisma
│   └── services
├── presentation
│   ├── controllers
│   ├── routes
│   └── middlewares
├── shared                 # Utilidades y excepciones
└── main.ts
```

Esta arquitectura permite:

- Separación clara de responsabilidades
- Bajo acoplamiento
- Escalabilidad
- Facilidad para pruebas y mantenimiento

### Frontend (React)

```bash
/src
├── application            # Casos de uso
├── domain                 # Entidades y contratos
├── infrastructure
│   ├── api
│   ├── repositories
│   └── services
├── presentation
│   ├── components
│   ├── pages
│   ├── hooks
│   └── layouts
├── shared
└── main.tsx
```

La arquitectura del frontend sigue los principios de Clean Architecture, facilitando la reutilización de componentes y la separación entre lógica de negocio e interfaz de usuario.

## Requisitos Previos

Asegúrate de tener instalado:

- Node.js >= 18
- NPM
- PostgreSQL

## Instalación

Clonar el repositorio:

```bash
git clone https://github.com/sebastian-alpizar/agricultural-management-system.git
cd agricultural-management-system
```

## Configuración del Backend

```bash
cd backend
npm install
```

Copiar y configurar el archivo `.env`:

```bash
cp .env.example .env
```

Editar `.env`:

```bash
DATABASE_URL=
PORT=
```

Ejecutar migraciones:

```bash
npx prisma migrate dev
```

Iniciar servidor:

```bash
npm run dev
```

## Configuración del Frontend

```bash
cd frontend
npm install
```

Copiar variables de entorno:

```bash
cp .env.example .env
```

Configurar:

```bash
VITE_API_URL=
```

Iniciar aplicación:

```bash
npm run dev
```

## Flujo del Sistema

1. Registrar trabajadores en el sistema.
2. Registrar asistencia diaria.
3. Asignar tareas y turnos según las necesidades operativas.
4. Monitorear productividad y rendimiento.
5. Calcular automáticamente pagos por horas trabajadas o productividad.
6. Generar reportes de eficiencia laboral y costos operativos.
7. Exportar información en PDF o Excel.
8. Facilitar la toma de decisiones mediante métricas y reportes.

## 📊 Ejemplos Visuales

```text
docs/images/dashboard.png
docs/images/workers.png
docs/images/reports.png
```

## Funcionalidades Clave

- Gestión de trabajadores
- Registro de asistencia
- Asignación de tareas
- Planificación de turnos
- Seguimiento de productividad
- Cálculo automático de pagos
- Reportes de eficiencia laboral
- Reportes de costos operativos
- Exportación a PDF
- Exportación a Excel
- Arquitectura limpia y escalable

## Despliegue

### Backend (Express)

- Railway
- Render
- VPS

Configurar:

- Variables de entorno
- Base de datos PostgreSQL

### Frontend (React)

Construir aplicación:

```bash
npm run build
```

Publicar en:

- Vercel
- Netlify

## Principios de Diseño

El proyecto implementa **Clean Architecture** tanto en backend como en frontend, siguiendo principios de:

- Separación de responsabilidades
- Bajo acoplamiento
- Inversión de dependencias
- Reutilización de código
- Escalabilidad
- Mantenibilidad
- Facilidad de pruebas

## Autor

**Desarrollado por Sebastián Alpízar Porras**

GitHub: https://github.com/sebastian-alpizar  
Email: sebastianalpiz@gmail.com
