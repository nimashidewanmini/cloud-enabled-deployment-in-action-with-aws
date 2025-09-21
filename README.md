
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

![Springboot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
[![React.js](https://img.shields.io/badge/React-000000?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![NPM](https://img.shields.io/badge/NPM-%23000000.svg?style=for-the-badge&logo=npm&logoColor=white)
![MySQL](	https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)

### 📌 Deploy & Containerize:

![AWS](https://img.shields.io/badge/AWS-000000?style=for-the-badge&logo=amazonaws&logoColor=FF9900)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)

### 📌 Demo Video:

- [watch](https://drive.google.com/file/d/10uWht31Oq65muZlBGeDhiayspYlo1HLW/view?usp=sharing)


### 📌 Clone the repository:

```bash
git clone https://github.com/nimashidewanmini/cloud-enabled-deployment-in-action-with-aws.git
```  



## 📌 License
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
