Overview
Task Manager is a full-stack web application designed to manage tasks with a clean UI and powerful backend. It demonstrates a well-rounded grasp of modern development tools and best practices, with a Python (Flask) backend and a JavaScript (React) frontend. The project is deployed on an AWS EC2 instance, simulating a real-world deployment environment.

This application allows users to:
•	Create, read, update, and delete (CRUD) tasks.
•	Visually distinguish completed tasks with styling.
•	Explore an API-driven frontend-backend architecture.


Tech Stack

Backend
•	Python: Primary backend language.
•	Flask: Lightweight framework to create RESTful APIs.
•	SQLAlchemy: ORM to interact with an SQLite database.
•	CORS: Enabled for cross-origin communication between frontend and backend.
•	Gunicorn: WSGI HTTP server for Python applications, used in production.
•	Unit Testing (Planned): Extend with pytest to test API endpoints.

Frontend
•	React: Component-based UI library for building dynamic interfaces.
•	Fetch API: To handle asynchronous requests to the backend.
•	Vite: Development server and bundler for improved speed and modularity.

Deployment
•	AWS EC2: Cloud virtual machine used to host the backend service.
•	SSH: Used to securely access and deploy to the EC2 instance.
•	Git/GitHub: Version control and collaborative development.

Folder Structure
taskmanager/
│
├── backend/
│   ├── app.py
│   ├── models.py
│   ├── requirements.txt
│   └── .env
│
├── frontend/
│   ├── src/
│   │   ├── App.js
│   │   ├── index.js
│   │   └── components/
│   └── vite.config.js
│
├── README.md


Setup Instructions

To clone the Repository… 
git clone https://github.com/your-username/taskmanager.git
cd taskmanager

Backend Setup

1.	Navigate to the backend folder:
cd backend

2.	Create and activate a virtual environment:
python3 -m venv venv
source venv/bin/activate

3.	Install dependencies:
pip install -r requirements.txt

4.	Run the Flask server:
python app.py

Frontend Setup

1.	Open a new terminal, navigate to the frontend directory:
cd frontend

2.	Install frontend dependencies:
npm install

3.	Run the React development server:
npm run dev

Deployment (AWS EC2)
1.	Launch an EC2 instance (Ubuntu).
2.	SSH into your instance using:
ssh -i your-key.pem ec2-user@your-ec2-ip
3.	Clone your GitHub repo and setup backend as above.
4.	Use gunicorn or similar for production server management.
5.	Configure security groups to allow port 5000/8000 for access.

Future Enhancements
•	Implement user authentication.
•	Add persistent database (e.g., PostgreSQL) using RDS.
•	Improve frontend design using TailwindCSS or Bootstrap.
•	Add comprehensive unit and integration tests.
•	Enable CI/CD pipelines via GitHub Actions.

Learning Goals
•	Full-stack web development experience.
•	Practical use of Git, GitHub, Flask, and React.
•	Understanding of RESTful API architecture.
•	Deployment to cloud infrastructure (AWS).
•	Debugging, testing, and local/prod environment management.

Jasmine Delens
Backend Engineer & Full Stack Developer
