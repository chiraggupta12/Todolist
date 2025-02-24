<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Todo List</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            max-width: 500px;
            margin: 0 auto;
            padding: 20px;
            color: #333;
        }
        
        h1 {
            text-align: center;
            color: #2c3e50;
        }
        
        .todo-container {
            background-color: #f9f9f9;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        
        #task-input {
            width: 70%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 16px;
        }
        
        #add-button {
            width: 25%;
            padding: 10px;
            background-color: #3498db;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        
        #add-button:hover {
            background-color: #2980b9;
        }
        
        ul {
            list-style-type: none;
            padding: 0;
            margin-top: 20px;
        }
        
        li {
            padding: 12px 20px;
            background-color: white;
            border-radius: 4px;
            margin-bottom: 8px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
        }
        
        .completed {
            text-decoration: line-through;
            color: #7f8c8d;
            background-color: #f8f9fa;
        }
        
        .task-text {
            flex-grow: 1;
            cursor: pointer;
        }
        
        .delete-btn {
            background-color: #e74c3c;
            color: white;
            border: none;
            border-radius: 4px;
            padding: 5px 10px;
            cursor: pointer;
            margin-left: 10px;
        }
        
        .delete-btn:hover {
            background-color: #c0392b;
        }
        
        .empty-list {
            text-align: center;
            color: #7f8c8d;
            font-style: italic;
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <div class="todo-container">
        <h1>My To-Do List</h1>
        
        <div>
            <input type="text" id="task-input" placeholder="Add a new task...">
            <button id="add-button">Add</button>
        </div>
        
        <ul id="task-list">
            <!-- Tasks will be added here -->
        </ul>
        
        <p id="empty-message" class="empty-list">No tasks yet. Add one above!</p>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const taskInput = document.getElementById('task-input');
            const addButton = document.getElementById('add-button');
            const taskList = document.getElementById('task-list');
            const emptyMessage = document.getElementById('empty-message');
            
            // Load tasks from localStorage
            let tasks = JSON.parse(localStorage.getItem('tasks')) || [];
            
            // Function to save tasks to localStorage
            function saveTasks() {
                localStorage.setItem('tasks', JSON.stringify(tasks));
                updateEmptyMessage();
            }
            
            // Function to update empty message visibility
            function updateEmptyMessage() {
                if (tasks.length === 0) {
                    emptyMessage.style.display = 'block';
                } else {
                    emptyMessage.style.display = 'none';
                }
            }
            
            // Function to render tasks
            function renderTasks() {
                taskList.innerHTML = '';
                
                tasks.forEach((task, index) => {
                    const li = document.createElement('li');
                    if (task.completed) {
                        li.classList.add('completed');
                    }
                    
                    const taskText = document.createElement('span');
                    taskText.classList.add('task-text');
                    taskText.textContent = task.text;
                    
                    // Toggle completion on click
                    taskText.addEventListener('click', function() {
                        tasks[index].completed = !tasks[index].completed;
                        saveTasks();
                        renderTasks();
                    });
                    
                    const deleteBtn = document.createElement('button');
                    deleteBtn.classList.add('delete-btn');
                    deleteBtn.textContent = 'Delete';
                    
                    // Delete task on click
                    deleteBtn.addEventListener('click', function() {
                        tasks.splice(index, 1);
                        saveTasks();
                        renderTasks();
                    });
                    
                    li.appendChild(taskText);
                    li.appendChild(deleteBtn);
                    taskList.appendChild(li);
                });
                
                updateEmptyMessage();
            }
            
            // Add new task
            function addTask() {
                const taskText = taskInput.value.trim();
                
                if (taskText !== '') {
                    tasks.push({
                        text: taskText,
                        completed: false
                    });
                    
                    saveTasks();
                    renderTasks();
                    taskInput.value = '';
                }
            }
            
            // Add task on button click
            addButton.addEventListener('click', addTask);
            
            // Add task on Enter key
            taskInput.addEventListener('keypress', function(e) {
                if (e.key === 'Enter') {
                    addTask();
                }
            });
            
            // Initial render
            renderTasks();
        });
    </script>
</body>
</html>
