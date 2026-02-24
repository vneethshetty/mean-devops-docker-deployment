In this DevOps task, you need to build and deploy a full-stack CRUD application using the MEAN stack (MongoDB, Express, Angular 15, and Node.js). The backend will be developed with Node.js and Express to provide REST APIs, connecting to a MongoDB database. The frontend will be an Angular application utilizing HTTPClient for communication.  

The application will manage a collection of tutorials, where each tutorial includes an ID, title, description, and published status. Users will be able to create, retrieve, update, and delete tutorials. Additionally, a search box will allow users to find tutorials by title.

## Project setup

### Node.js Server

cd backend

npm install

You can update the MongoDB credentials by modifying the `db.config.js` file located in `app/config/`.

Run `node server.js`

### Angular Client

cd frontend

npm install

Run `ng serve --port 8081`

You can modify the `src/app/services/tutorial.service.ts` file to adjust how the frontend interacts with the backend.

Navigate to `http://localhost:8081/`

## 📸 Screenshots

### 🔹 GitHub Actions - Successful Pipeline
![GitHub Actions](screenshots/github-actions-success.png)

### 🔹 Docker Hub Images
![Docker Hub](screenshots/dockerhub-images.png)

### 🔹 AWS EC2 Instance
![AWS EC2](screenshots/aws-ec2-instance.png)

### 🔹 Live Application (Public IP)
![Live App](screenshots/live-application.png)

### 🔹 API Response
![API Response](screenshots/api-response.png)

### 🔹 Nginx Reverse Proxy Configuration
![Nginx Config](screenshots/nginx-config.png)