##Permalist: A Persistent To-Do List Application 📝
     Permalist is a simple yet efficient to-do list application that lets users manage their tasks with ease. Unlike temporary lists, Permalist ensures that your tasks are stored in a 
     database, so your progress is never lost.

#Features 🚀
  . Add Tasks: Add new tasks to your to-do list.
  . Edit Tasks: Update task titles as needed.
  . Delete Tasks: Remove completed or unwanted tasks.
  . Persistent Storage: All tasks are stored in a PostgreSQL database for long-term access.
  . User-Friendly Interface: A clean and intuitive design for task management.
**How It Works 🔧**
  . Backend:
     Built using Node.js and Express.js, Permalist handles user interactions efficiently.
     Data is stored in a PostgreSQL database for persistence.

  . Frontend:
     Renders a dynamic to-do list using EJS for templates, allowing seamless interaction with tasks.

  . Database:
     PostgreSQL stores all tasks with their unique IDs and titles for easy retrieval and updates.

**Technologies Used 🛠️**
  . Node.js: For server-side scripting.
  . Express.js: For building the backend RESTful API.
  . PostgreSQL: For database management.
  . EJS: For rendering dynamic web pages.
  . Body-Parser: For handling form data.
  . CSS: For styling the application.
  . Setup Instructions 🖥️
#Clone the repository:
    ```bash
         git clone https://github.com/Mohammed-Farida23/Permalist.git
          cd Permalist
 #Install dependencies:
    ```bash
         npm install```
#Configure the database:

  . Ensure you have PostgreSQL installed and running.
  . Create a database named Permalist.
  . Add an items table using the following SQL query:
       ```sql
             CREATE TABLE items (
              id SERIAL PRIMARY KEY,
              title TEXT NOT NULL
              );```


#Update database credentials:
      . Open index.js and update the database configuration:
  ```javascript
       const db = new pg.Client({
       user: "your_username",
        host: "localhost",
        database: "Permalist",
        password: "your_password",
       port: 5432,
    });

  #Run the application:
 bash
          node index.js
          Access the app:
          Open your browser and visit http://localhost:3000.

     #Project Structure 📂
   php

     Permalist/
     ├── public/             # Static files (CSS, images)
     ├── views/              # EJS templates
     │   └── index.ejs       # Main UI
     ├── index.js            # Main server file
     ├── package.json        # Project metadata and dependencies
     └── README.md           # Project documentation





**Future Enhancements 🌟**
  . Add user authentication for personalized task lists.
  . Implement task categories or priorities.
  . Enhance styling for a more modern design.
  . Add due dates and reminders for tasks.
  . Integrate APIs for advanced features (e.g., sharing tasks or syncing with calendars).
##License 📜
    This project is licensed under the MIT License. Feel free to use, modify, and share it.

