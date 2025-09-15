Todo List CRUD Application
A simple web-based Todo List application that implements Create, Read, Update, and Delete (CRUD) operations. Built with React, Tailwind CSS, and a JSON server backend, this app allows users to manage their tasks efficiently.
Description
The Todo List CRUD Application is designed for personal task management. It features an intuitive interface where users can add new todos, view their list, edit existing items, mark them as completed, and delete them as needed. The app uses a local JSON server for data persistence, making it easy to set up and test.
Features

Create: Add new todo items via an input field.
Read: Display all todos with a clear distinction for completed tasks (struck through).
Update: Edit todo titles and save changes.
Delete: Remove todos with a single click.
Toggle Completion: Mark todos as completed or incomplete with checkboxes.

Prerequisites

Node.js: Version 14.x or later (recommended).
npm: Comes with Node.js installation.
json-server: For the backend API.

Installation

Clone the Repository
git clone https://github.com/your-username/todo-crud-app.git
cd todo-crud-app


Install Dependencies

For the frontend (Vite + React):npm install


Install json-server globally (if not already installed):npm install -g json-server




Set Up the Backend

Ensure a db.json file exists in the project root with the following content:{
  "todos": []
}


Start the JSON server:json-server --watch db.json --port 3000




Run the Application

Start the development server:npm run dev


Open your browser and navigate to http://localhost:5173 (or the port specified by Vite).



Usage

Add a Todo: Enter a task in the input field and click "Add Todo".
View Todos: The list displays all tasks, with completed ones struck through.
Edit a Todo: Click "Edit" on a todo, modify the text, and click "Save".
Delete a Todo: Click "Delete" to remove a todo.
Toggle Completion: Check the box to mark a todo as completed.

Sample Todo List
To pre-populate the app, update db.json with:
{
  "todos": [
    { "id": 1, "title": "Buy groceries", "completed": false },
    { "id": 2, "title": "Finish homework", "completed": false },
    { "id": 3, "title": "Call mom", "completed": true },
    { "id": 4, "title": "Exercise", "completed": false },
    { "id": 5, "title": "Read a book", "completed": true }
  ]
}

Save the file, and the JSON server will reflect the changes.
Project Structure

src/: Contains React components and styles.
App.jsx: Main application component.
index.css: Tailwind CSS directives.
main.jsx: Entry point for React rendering.


index.html: Base HTML file (used with Vite).
db.json: Backend data file.
tailwind.config.js: Tailwind CSS configuration.
package.json: Project dependencies and scripts.

Technologies Used

Frontend: React, Tailwind CSS, Vite, Axios.
Backend: JSON Server.
Styling: Tailwind CSS (installed via PostCSS for production readiness).

Contributing

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit them (git commit -m "description").
Push to the branch (git push origin feature-branch).
Open a pull request.

License
This project is open-source and available under the MIT License.
Acknowledgements

Inspired by the need for a simple CRUD example.
Built with guidance from xAI's Grok.

Contact
For questions or support, please open an issue on the GitHub repository.
