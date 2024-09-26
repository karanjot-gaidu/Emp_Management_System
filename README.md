# Employee Managemeent System (EMS)

This project is an Employee Management System (EMS) that consists of two main components:

- Backend: Developed using Spring Boot.
- Frontend: Developed using Vite.js.

Both the backend and frontend are located in separate folders, namely ems-backend and ems-frontend, and need to be run separately.

## Prerequisites
Before you begin, ensure you have the following installed on your system:

- Java 17 or higher (for running the Spring Boot backend)
- Node.js and npm (for running the Vite.js frontend)
- MySQL or another compatible relational database system (for the EMS database)

## Setup Instructions
### 1. Clone the Repository
```bash
git clone https://github.com/karanjot-gaidu/Emp_Management_System.git
```
### 2. Backend Setup (Spring Boot)
1. Navigate to the `ems-backend` folder:
    ```bash
    cd ems-backend
    ```
2. Create a database named ems in MySQL or your preferred database system.

3. Configure your database connection in the application.properties file located in the src/main/resources/ directory. Update the following fields:
    ```java
    spring.datasource.url=jdbc:mysql://localhost:3306/ems
    spring.datasource.username=your_db_username
    spring.datasource.password=your_db_password
    ```
4. Build and run the backend application:
    ```bash
    ./mvnw spring-boot:run
    ```
    Alternatively, you can run the EmployeeManagementApplication class directly if you’re using an IDE like IntelliJ IDEA or Eclipse.

### 3. Frontend Setup (Vite.js)
1. Navigate to the `ems-frontend` folder:
    ```bash
    cd ems-frontend
    ```

2. Install the necessary npm packages:
    ```bash
    npm install
    ```

3. Start the development server:
    ```bash
    npm run dev
    ```

4. The frontend should now be accessible in your browser at:
    ```
    http://localhost:5173
    ```

## Additional Information
- Backend API: The Spring Boot backend exposes a RESTful API. Ensure the backend is running before accessing the frontend.

- Frontend Access: The frontend interacts with the backend via API calls. Make sure the backend is up and running to avoid any connection issues.