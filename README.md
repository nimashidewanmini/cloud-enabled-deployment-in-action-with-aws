
# Cloud Enabled Deployment In Action

## Introduction
This repository highlights a cloud-powered ☁️ microservices architecture built with Spring Boot 🍃, React ⚛️, AWS 🟨, GCP 🔵, and Docker 🐳. It demonstrates how to develop 🛠️, containerize 📦, and deploy 🚢 both backend services and a frontend app, leveraging a mix of cloud-managed 🌐 and self-hosted 🖥️ databases.
The repository is organized into four main projects:

- course-service → Spring Boot + MySQL

- student-service → Spring Boot + MongoDB

- media-service → Spring Boot + local file storage (extensible to S3/MinIO)

- frontend-app → React + TypeScript


## Backend Services

**1.** **course-service:**

- Entity: Course(id, name, duration)
- Endpoints:

  - GET /courses
  - GET /courses/{id}
  - POST /courses
  - DELETE /courses/{id}

- Default Port: 8081

- Configuration: Connects to MySQL

**2.** **student-service:**

- Document: Student(registrationNumber, fullName, address, contact, email)

- Endpoints:

  - GET /students

  - GET /students/{id}

  -  POST /students

  -  DELETE /students/{id}

- Default Port: 8082

- Configuration: Uses MongoDB

**3.** **media-service:**

- Resource: files

- Endpoints:

  - POST /files → upload (multipart/form-data)

  - GET /files → list all files

  - GET /files/{id} → fetch file

  - DELETE /files/{id} → delete file

- Default Port: 8083

## Frontend (frontend-app)

- Stack: React + TypeScript + MUI + Axios + Vite

- Sections: Courses | Students | Media

- Scripts:

  - npm run dev → Start Vite dev server

  -  npm run build → Compile TypeScript + Vite build

  - npm run preview → Preview production build


### Build

- Backend: Run
```bash
mvn -q -e -DskipTests package

``` 
- Frontend: Run
```bash
npm install
npm run dev

``` 
### 📌 Build with

- Spring Boot 🍃

- React.js ⚛️

- TypeScript 🔷

- Node.js 🟩

- NPM 📦

- MySQL 🟨

- MongoDB 🟦

### 📌 Deploy & Containerize:

- AWS ☁️

- Google Cloud 🔵

- Docker 🐳

### 📌 Demo Video:

- [watch](https://drive.google.com/file/d/10uWht31Oq65muZlBGeDhiayspYlo1HLW/view?usp=sharing)


### Clone the repository:

```bash
git clone https://github.com/nimashidewanmini/cloud-enabled-deployment-in-action-with-aws.git
```  



## License
This project is licensed under the MIT License - see the [MIT License](LICENSE) file for details.

<br>

<br>

## 📄 Student Information

- **Name:** Nimashi Dewanmini
- **Registration Number:** 2301682013
- **Email Address:** nimashidewanmini@gmail.com

<br>


<p align="center">
  &copy; 2024 Nimashi Dewanmini
</p>
