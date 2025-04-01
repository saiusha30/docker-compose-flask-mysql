# Flask & MySQL with Docker Compose

A simple Flask app with a MySQL database, running in Docker using Docker Compose.

## Features
- Flask web application
- MySQL database
- Docker Compose for container orchestration

## Prerequisites
Ensure you have the following installed:
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Git](https://git-scm.com/)

## Project Structure
```
flask-mysql-docker/
│── app/
│   ├── app.py
│   ├── requirements.txt
│   ├── Dockerfile
│── docker-compose.yml
│── .gitignore
│── README.md
```

## Setup Instructions
### 1. Clone the Repository
```bash
git clone git@github.com:saiusha30/docker-compose-flask-mysql.git

cd flask-mysql-docker
```

### 2. Build and Run Containers
```bash
docker-compose up --build (incase it is not work use this below
docker compose up -d

```
### To list the containers
docker compose ps


### 3. Access the Application
- The Flask app runs on **http://localhost:5000**.
- MySQL database is accessible on port **3306** with:
  - **Database Name:** `flaskdb`
  - **User:** `flaskuser`
  - **Password:** `flaskpassword`

### 4. Stopping the Containers
To stop the running containers:
```bash
docker compose down
```

## Explanation of Files
- **app/app.py**: Flask application code.
- **app/requirements.txt**: Python dependencies.
- **app/Dockerfile**: Docker configuration for Flask.
- **docker-compose.yml**: Defines and manages multi-container applications.
- **.gitignore**: Files to exclude from Git version control.

## Push to GitHub
```bash
git add .
git commit -m "Initial commit: Flask & MySQL with Docker Compose"
git push -u origin main
```

## Author
ushaparvathina
https://github.com/saiusha30


