# Cloud Enabled Deployment In Action with AWS And Azure

This repository contains four projects:

- **course-service** (Spring Boot + MySQL)
- **student-service** (Spring Boot + MongoDB)
- **media-service** (Spring Boot + Local file storage, can be extended to S3/MinIO)
- **frontend-app** (React + TypeScript)

---

## Backend Services

### 1. course-service (AWS & Azure)
- **Entity**: `Course(id, name, duration)`
- **Endpoints**:
    - `GET /courses`
    - `GET /courses/{id}`
    - `POST /courses`
    - `DELETE /courses/{id}`
- **Default port**: 8081
- Configure MySQL settings.

### 2. student-service (AWS)
- **Document**: `Student(registrationNumber, fullName, address, contact, email)`
- **Endpoints**:
    - `GET /students`
    - `GET /students/{id}`
    - `POST /students`
    - `DELETE /students/{id}`
- **Default port**: 8082
- Configure MongoDB settings.

### 3. media-service
- **Resource**: `files`
- **Endpoints**:
    - `POST /files` (multipart/form-data: file)
    - `GET /files` (list)
    - `GET /files/{id}` (fetch)
    - `DELETE /files/{id}` (delete)
- **Default port**: 8083
- Uses local disk storage at `./data/media` by default (override with `MEDIA_STORAGE_DIR` environment variable).

---

## Frontend (frontend-app)

- **Stack**: React + TypeScript + MUI + Axios + Vite
- **Sections**: Courses, Students, Media
- **Scripts**:
    - `npm run dev` – Vite dev server
    - `npm run build` – TypeScript + Vite build
    - `npm run preview` – Preview built app
    - 

## Azure Deployment (Course-service)

- **Name**: K.G Kavindu Madhuranga Wijerathna
- **Student ID**: 2301671008
- **Email**: kavindumaduranga184@gmail.com
- **GitHub Repository**: https://github.com/kavindu0818/azure-sql-springboot-application.git
- **Demo Video**: https://drive.google.com/file/d/1bdmV0yugqMgxHA4crJfsxqmvMtRmmLZG/view?usp=sharing
