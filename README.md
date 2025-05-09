# Tienda Electrónica Full-Stack

**Tienda electrónica full-stack con Node.js, Express, TypeScript y Angular para vender productos 3D, hardware de minería Bitcoin y soluciones Smart Home.**

---

## 🏷️ Tecnologías

* **Backend:** Node.js, Express, TypeScript, Mongoose/Prisma
* **Frontend:** Angular 16+, TypeScript, RxJS, HttpClient
* **Autenticación:** JWT, bcryptjs
* **Base de Datos:** MongoDB Atlas o PostgreSQL (RDS)
* **Infraestructura:** Heroku / Azure / AWS
* **CI/CD:** GitHub Actions

---

## 📁 Estructura del Monorepo

```
/tienda-electronica-fullstack
├── README.md           # Documentación del proyecto
├── .gitignore
├── backend             # API con Node.js + Express + TypeScript
│   ├── src
│   │   ├── controllers
│   │   ├── models
│   │   ├── routes
│   │   ├── middlewares
│   │   └── index.ts
│   ├── tsconfig.json
│   ├── package.json
│   └── .env.example
│
└── frontend            # Aplicación Angular
    ├── src
    │   ├── app
    │   │   ├── components
    │   │   ├── services
    │   │   ├── models
    │   │   ├── pages
    │   │   └── app.module.ts
    │   ├── assets
    │   └── environments
    ├── angular.json
    ├── tsconfig.json
    ├── package.json
    └── .env.example
```

---

## 🚀 Comenzando

### Prerrequisitos

* Node.js >=18
* npm o yarn
* Angular CLI `npm install -g @angular/cli`
* Cuenta MongoDB Atlas o servidor PostgreSQL

### Instalación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/gpalomino91/tienda-electronica-fullstack.git
   cd tienda-electronica-fullstack
   ```

2. Instala dependencias del backend:

   ```bash
   cd backend
   npm install
   ```

3. Configura variables de entorno en `backend/.env` (copia `.env.example`):

   ```ini
   DB_URI=<tu_URI_de_BD>
   JWT_SECRET=<tu_secreto>
   PORT=4000
   ```

4. Instala dependencias del frontend:

   ```bash
   cd ../frontend
   npm install
   ```

5. Configura `frontend/.env` si hace falta:

   ```ini
   API_URL=http://localhost:4000/api
   ```

---

## 🛠️ Uso en Desarrollo

1. Levanta el backend en modo desarrollo:

   ```bash
   cd backend
   npm run dev
   ```

2. Arranca el frontend:

   ```bash
   cd frontend
   ng serve
   ```

3. Abre en el navegador `http://localhost:4200`

---

## 🔧 Pruebas

* **Backend:**

  ```bash
  cd backend
  npm test
  ```
* **Frontend:**

  ```bash
  cd frontend
  ng test
  ```

---

## 🚢 Despliegue

1. Configura variables de entorno en tu servicio (Heroku, Azure, AWS).
2. En GitHub Actions está configurado el flujo CI para build y tests.
3. Deploy automático tras merge a `main`.

---

## 🤝 Contribuciones

1. Haz fork del repositorio
2. Crea una rama: `git checkout -b feature/nueva-funcionalidad`
3. Realiza commits: `git commit -m "Agrega feature"`
4. Push: `git push origin feature/nueva-funcionalidad`
5. Abre un Pull Request

---

## 📜 Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.
