# Resume Analyzer

This project is a full-stack application for analyzing resumes and matching them with job descriptions. It consists of three main components:
1. **Backend (Spring Boot)**: Handles authentication, resume/job description uploads, and matching logic.
2. **Frontend (React)**: Provides a user interface for interacting with the application.
3. **AI Service (Flask)**: Performs resume analysis and matching using machine learning.

---

## Prerequisites

Ensure the following are installed on your system:
- **Java 21** (for the backend)
- **Maven** (for building the backend)
- **Node.js** and **npm** (for the frontend)
- **Python 3.9+** (for the AI service)
- **PostgreSQL** (for the database)

---

## Setup Instructions

### 1. Backend (Spring Boot)
1. Navigate to the backend directory:
   ```bash
   cd /Users/saicharan/Desktop/my proj/resume-analyzer
   ```
2. Configure the database:
   - Update the `application.properties` file in `src/main/resources` with your PostgreSQL credentials.
   - Example:
     ```properties
     spring.datasource.url=jdbc:postgresql://localhost:5432/resume
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     ```
3. Build and run the backend:
   ```bash
   ./mvnw spring-boot:run
   ```
4. The backend will start on `http://localhost:8080`.

---

### 2. Frontend (React)
1. Navigate to the frontend directory:
   ```bash
   cd /Users/saicharan/Desktop/my proj/frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
4. Open the frontend in your browser at `http://localhost:5173`.

---

### 3. AI Service (Flask)
1. Navigate to the AI service directory:
   ```bash
   cd /Users/saicharan/Desktop/my proj/ai
   ```
2. Create a virtual environment and activate it:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Flask app:
   ```bash
   python app.py
   ```
5. The AI service will start on `http://localhost:6000`.

---

## Running the Application
1. Start the backend, frontend, and AI service as described above.
2. Open the frontend in your browser (`http://localhost:5173`) and interact with the application.

---

## Notes
- Ensure all services are running simultaneously.
- Use the same PostgreSQL database for the backend.
- For any issues, check the logs of each service for debugging.

Enjoy using the Resume Analyzer!
