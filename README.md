# Medicare — Healthcare Appointment Platform

A full-featured healthcare web app with three portals built with React, Vite, TypeScript, and Tailwind CSS.

![App Preview](public/opengraph.jpg)

## Portals

- **Patient** — Browse doctors, book appointments, manage profile
- **Admin** — Dashboard, manage appointments and doctors (`/admin`)
- **Doctor** — Dashboard, view appointments, update profile (`/doctor`)

## Getting Started

```bash
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

## Build for Production

```bash
npm run build
npm run preview
```
## Folder structure

```
Medicare/
├── backend/                  # Backend API & Server logic
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/medicare/
│   │   │   │   ├── controllers/      # Route handlers (e.g., PatientController, DoctorController)
│   │   │   │   ├── models/           # Database schemas/entities (e.g., Patient, Appointment)
│   │   │   │   ├── repositories/     # Database access layer
│   │   │   │   ├── services/         # Business logic
│   │   │   │   ├── security/         # Authentication & Authorization (JWT, etc.)
│   │   │   │   └── MedicareApplication.java # Main application entry point
│   │   │   └── resources/
│   │   │       ├── application.properties # DB configs, port settings
│   │   │       ├── static/            # Static assets (if serving frontend from backend)
│   │   │       └── templates/         # Email templates, older JSP/Thymeleaf views
│   │   └── test/                      # Backend unit and integration tests
│   ├── pom.xml                        # Maven dependencies (if Java) or package.json (if Node)
│   └── README.md
│
├── frontend/                 # Client-side Application
│   ├── public/
│   │   ├── index.html        # Main HTML file
│   │   ├── favicon.ico
│   │   └── assets/           # Global images, icons, and static CSS
│   ├── src/
│   │   ├── components/       # Reusable UI components
│   │   │   ├── Navbar/
│   │   │   ├── Footer/
│   │   │   ├── PatientCard/
│   │   │   └── AppointmentForm/
│   │   ├── pages/            # Main application views
│   │   │   ├── Home/
│   │   │   ├── AdminDashboard/
│   │   │   ├── DoctorPortal/
│   │   │   ├── PatientProfile/
│   │   │   └── Login/
│   │   ├── services/         # API call functions (e.g., api.js, auth.service.js)
│   │   ├── styles/           # Global stylesheets
│   │   ├── utils/            # Helper functions and constants
│   │   ├── App.js            # Main React/Angular/Vue component
│   │   └── index.js          # Frontend entry point
│   ├── package.json          # Frontend dependencies
│   └── .env                  # Environment variables (API endpoints)
│
├── database/                 # Database initialization scripts
│   ├── schema.sql            # Table creation scripts
│   └── data.sql              # Dummy data for testing
│
├── docs/                     # Project documentation
│   ├── api-endpoints.md
│   ├── system-architecture.png
│   └── setup-guide.md
│
├── .gitignore
├── docker-compose.yml        # Container orchestration (optional)
└── README.md                 # Root documentation

```


## Demo Credentials

| Portal | Email | Password |
|--------|-------|----------|
| Admin  | admin@medicare.com | password123 |
| Doctor | doctor@medicare.com | password123 |

> All data is mocked — no backend required.

## Tech Stack

- React 19 + TypeScript
- Vite 7
- Tailwind CSS v4
- React Router v7
- shadcn/ui components
- React Toastify
