# 👨‍💼 Employee Offboarding System

## Overview

🚀 The **Employee Offboarding System** is an Angular-based web application designed to help organizations manage **employee offboarding**, track assigned equipment, and update employee statuses. The application is built with **Angular CLI 19.2.3**, **Angular Material**, and **JSON Server** for mock API functionality.

## Prerequisites

- **Node.js (v18+)** → [Download](https://nodejs.org/)
- **Angular CLI (v19+)** → Install via:
  ```sh
  npm install -g @angular/cli
  ```
- **JSON Server (for mock API)**
  ```sh
  npm install -g json-server
  ```

## Setup

### 1️⃣ **Clone the Repository**
```sh
git clone https://github.com/bartlomiej-629/employee-offboarding.git
cd employee-offboarding
```

### 2️⃣ **Install Dependencies**
```sh
npm install
```

### 3️⃣ **Start JSON Server (Mock API)**
```sh
npx json-server --watch src/assets/mock-server/db.json --port 3000 --host 127.0.0.1
```
🔹 This will run the **mock API** at `http://127.0.0.1:3000/employees`.

### 4️⃣ **Run the Angular App**
```sh
ng serve
```
🔹 The app will start at **`http://localhost:4200/`**.

## Usage

### **Dashboard Page**
- Displays the **list of employees** with search functionality.
- Clicking on an employee **navigates to the detailed page**.

### **Employee Details Page**
- Shows detailed **employee information**.
- Displays **assigned equipment** and **offboarding status**.

## Features

✔️ **Employee List with Search**  
✔️ **View Employee Details**  
✔️ **Track Equipment Assigned to Employees**  
✔️ **Update Offboarding Status**  
✔️ **Responsive UI (Desktop & Mobile)**  
✔️ **Mock API using JSON Server**  

## Approach and Methods

### **Employee Data Management**
- The **employee list** and details are fetched from `JSON Server` (`http://127.0.0.1:3000/employees`).
- `HttpClient` is used to interact with the **mock API**.

### **Navigation**
- The application **uses Angular Routing** to navigate between pages:
  - **Dashboard** → `http://localhost:4200/`
  - **Employee Details** → `http://localhost:4200/employee/:id`

### **Search Functionality**
- Employees can be **filtered** dynamically as the user types in the search field.

### **Styling & Design**
- **Angular Material** components are used for UI consistency.
- The **employee table** is responsive, with a hover effect to indicate clickable rows.

### **API Calls & Data Handling**
- The `EmployeeService` is responsible for:
  - Fetching employees
  - Getting employee details
  - Updating offboarding status

## Technologies Used

| Tech | Description |
|------|------------|
| [Angular 19](https://angular.io/) | Frontend Framework |
| [TypeScript](https://www.typescriptlang.org/) | Programming Language |
| [Angular Material](https://material.angular.io/) | UI Components |
| [JSON Server](https://github.com/typicode/json-server) | Mock API for Backend |

## Points for Improvement

1. **Error Handling:** Improve API error handling and display user-friendly messages.
2. **Logging:** Implement logging for better debugging.
3. **Real Backend Integration:** Replace JSON Server with a real backend API.
4. **Security:** Store API keys securely in environment variables.
5. **Testing:** Add unit and integration tests using Jasmine/Karma.

### 🎉 **Thank You for Using Employee Offboarding System!** 🚀

