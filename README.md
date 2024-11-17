
# Task Manager App

## 1. Application Overview and Functionality

The **Task Manager App** is a simple to-do list application built using React. It allows users to:

- **Add a task**: Enter a task in the input field and click the "Add Task" button to add it to the task list.
- **Delete a task**: Click the "Delete" button next to each task to remove it from the list.
- **Persistent storage**: Tasks are saved in the browser's local storage, so they persist even after a page refresh.
- **Visuals**: Tasks are displayed with a light blue background and can be removed via a red "Delete" button. The "Add Task" button is disabled when the input field is empty, with a "not-allowed" cursor to indicate that adding tasks is not permitted until input is provided.

### Features:
- Add tasks to a list.
- Delete tasks from the list.
- Persist tasks using **localStorage**.
- Clear and user-friendly interface with a dynamic button state (disabled when input is empty).

---

## 2. Setup and Launch Process

Follow the steps below to set up and run the Task Manager App locally on your system.

### Requirements:
- Node.js (version 14 or higher)
- npm (Node Package Manager)

### Steps:

1. **Clone the Repository:**

   First, clone the repository to your local machine using the following command:

   ```bash
   git clone https://github.com/yourusername/task-manager-app.git
   ```

2. **Install Dependencies:**

   Navigate to the project directory and install the required dependencies:

   ```bash
   cd task-manager-app
   npm install
   ```

3. **Run the Application:**

   Once the dependencies are installed, start the development server:

   ```bash
   npm start
   ```

   This will start the app on [http://localhost:3000](http://localhost:3000).

4. **Access the App:**

   Open a web browser and go to `http://localhost:3000`. You should now see the Task Manager App running locally.

---

## 3. Assumptions Made During Development

1. **No User Authentication**: This application does not require user authentication. It is a simple single-user to-do list.
   
2. **Tasks Stored in LocalStorage**: Tasks are stored in the browser's local storage. This means that tasks will persist between page reloads but will be cleared if the user clears their browser's local storage.

3. **Single Page Application (SPA)**: The app assumes it's being run as a single-page application, meaning no server-side rendering or complex routing is required.

4. **Basic Input Validation**: The application assumes that tasks entered are text and that no special characters or validation is needed beyond checking for an empty input field.

5. **Responsive Design**: While the design is responsive to some extent, it's optimized for mobile-first use but may need further adjustments for different screen sizes or additional features.

---

## 4. Screenshots

Below are some screenshots of the Task Manager App:

- **Task Added:**
  ![Task Added](/public/screenshots/task-added.png)

- **Empty Input State:**
  ![Empty Input](/public/screenshots/empty-input.png)

---
