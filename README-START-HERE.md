# Banking Management System - Local Setup

This version has a shorter folder structure so Windows and IntelliJ can see all Java files.

## 1. Create the database

Open MySQL Workbench, connect to `Local instance MySQL80`, and run the contents of `database-setup.sql`.

## 2. Run the Java backend in IntelliJ

1. In IntelliJ, select **File > Open**.
2. Open `backend/pom.xml` as a Maven project.
3. Set the Project SDK to **Java 17**.
4. Open this file:

   `backend/src/main/java/com/bankingSystem_Api/Full_Stack_BankingSystem_API/FullStackBankingSystemApiApplication.java`

5. Click the green run arrow beside `main`.

If your MySQL `root` account has a password, use **Run > Edit Configurations** and add this environment variable:

`DB_PASSWORD=your_mysql_password`

The backend runs at `http://localhost:8080`.

## 3. Run the React frontend

Open IntelliJ Terminal in the `frontend` folder and run:

```powershell
npm install
npm run dev
```

Open `http://localhost:5173` in your browser.

The frontend is already configured to use the local backend.
