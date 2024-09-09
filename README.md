minimalistic Full Stack App, with these technologies:
- nextjs 14
- Flask 
- SQLAlchemy
- PostgreSQL
- Docker
- Docker Compose
•   Post man to test http


Certainly! Here's a list of the main commands used throughout the workshop, organized by the different stages of the project:
	1. Project Setup: 

Copy
mkdir full-stack-flask-next
cd full-stack-flask-next
git init
touch .gitignore
touch compose.yml
	2. Database Setup (in compose.yml): 

Copy
docker compose up -d db
docker ps
docker exec -it db psql -U postgres
	3. Backend (Flask) Setup: 

Copy
mkdir backend
cd backend
touch requirements.txt
touch app.py
touch Dockerfile
	4. Building and Running the Backend: 

Copy
docker compose build flask
docker compose up -d flask
	5. Frontend (Next.js) Setup: 

Copy
npx create-next-app@latest frontend
cd frontend
npm install axios
npm run dev
	6. Creating Frontend Components: 

Copy
mkdir src/components
touch src/components/CardComponent.tsx
touch src/components/UserInterface.tsx
	7. Docker Setup for Frontend: 

Copy
touch .dockerignore
touch Dockerfile
	8. Building and Running the Full Stack: 

Copy
docker compose build
docker compose up -d
	9. Useful Docker Commands: 

Copy
docker ps
docker logs <container_name>
docker exec -it <container_name> /bin/sh
	10. npm Commands: 

Copy
npm install
npm run dev
npm audit fix
npm audit
npm audit fix --force
	11. Database Queries (inside PostgreSQL container): 

Copy
SELECT * FROM users;
	12. Git Commands: 

Copy
git add .
git commit -m "Your commit message"
git push
	13. Checking Installations: 

Copy
docker --version
python --version
node --version
npm --version
pip list | grep Flask
npm list next
![image](https://github.com/user-attachments/assets/1b7e06ec-ed1b-43c4-bb64-5b64afd7bb8f)
