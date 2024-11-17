# To-Do List Manager

Create a simple console application to manage a list of tasks. Uses can add, remove, and view their tasks.

### **Description and Working Procedure**

The **To-Do List Manager** is a console-based Java application designed to help users manage their tasks. The application allows users to add tasks, view the list of tasks, remove specific tasks, and exit the program when done. Below is a detailed breakdown of its functionality and working.

---

### **1. Purpose of the Program**
The program serves as a simple task manager that helps users keep track of their daily tasks. It enables users to:
- Add tasks to a list.
- View the tasks in an organized manner.
- Remove tasks based on their position in the list.
- Exit the program when all tasks are managed.

This application demonstrates basic programming concepts such as user input, list manipulation, and control structures in Java.

---

### **2. Key Components of the Code**
1. **Task Storage**:
   - The program uses an `ArrayList<String>` to store the tasks.  
   - An `ArrayList` is dynamic, meaning tasks can be added or removed without the need to predefine the size.

2. **User Input**:
   - The `Scanner` class is used to take input from the user, ensuring an interactive experience.

3. **Menu System**:
   - A `do-while` loop ensures that the menu is repeatedly displayed until the user chooses to exit.

4. **Switch-Case Logic**:
   - The menu options are handled using a `switch` statement.  
   - Each case corresponds to a specific functionality:
     - **Case 1**: Add a task.
     - **Case 2**: View tasks.
     - **Case 3**: Remove a task.
     - **Case 4**: Exit the program.

5. **Validation**:
   - The program checks for edge cases, such as:
     - Empty task lists when viewing or removing tasks.
     - Invalid task numbers for removal.

---

### **3. Working Procedure**
1. **Program Initialization**:
   - The program begins by initializing an empty `ArrayList` to store tasks.
   - A `Scanner` is also initialized for user input.

2. **Displaying the Menu**:
   - A menu with options (Add Task, View Tasks, Remove Task, Exit) is displayed to the user.
   - The user is prompted to choose an option by entering a number.

3. **Processing User Choice**:
   - Based on the user’s choice, the corresponding action is executed:
     - **Option 1 (Add Task)**:
       - Prompts the user to enter a task.
       - The entered task is added to the `ArrayList`.
       - A confirmation message is displayed.
     - **Option 2 (View Tasks)**:
       - Checks if the task list is empty.
       - If tasks exist, they are displayed in a numbered list format.
       - If no tasks exist, a message is shown indicating that the list is empty.
     - **Option 3 (Remove Task)**:
       - Checks if the task list is empty.
       - If tasks exist, displays the list and prompts the user to enter the number of the task to be removed.
       - Validates the entered number to ensure it corresponds to an existing task.
       - Removes the task and displays a confirmation message.
       - If the number is invalid, an error message is shown.
     - **Option 4 (Exit)**:
       - Displays a goodbye message and exits the program.

4. **Repeating the Process**:
   - The menu is displayed again after every operation until the user chooses to exit.

5. **Closing the Scanner**:
   - Before exiting, the `Scanner` is closed to free up resources.

---

### **4. Example Workflow**

#### Adding a Task:
```
--- To-Do List Manager ---
1. Add Task
2. View Tasks
3. Remove Task
4. Exit
Enter your choice: 1
Enter task: Complete homework
Task added!
```

#### Viewing Tasks:
```
--- To-Do List Manager ---
1. Add Task
2. View Tasks
3. Remove Task
4. Exit
Enter your choice: 2

Your Tasks:
1. Complete homework
```

#### Removing a Task:
```
--- To-Do List Manager ---
1. Add Task
2. View Tasks
3. Remove Task
4. Exit
Enter your choice: 3

Your Tasks:
1. Complete homework
Enter task number to remove: 1
Task removed!
```

#### Exiting the Program:
```
--- To-Do List Manager ---
1. Add Task
2. View Tasks
3. Remove Task
4. Exit
Enter your choice: 4
Exiting... Goodbye!
```

---

### **5. Key Features**
- **Dynamic Task Management**:
  - Tasks can be added or removed easily due to the flexibility of `ArrayList`.
- **Interactive Menu**:
  - The program provides a user-friendly menu for easy navigation.
- **Error Handling**:
  - Checks for empty lists and invalid inputs, ensuring robustness.

---

### **6. Practical Applications**
This program can be used as a basic task manager. It also serves as an excellent exercise for learning:
- ArrayList manipulation.
- Control flow with loops and conditionals.
- User input validation.

---

### **Conclusion**
The **To-Do List Manager** is a simple yet powerful tool for managing tasks in a console-based environment. It introduces core programming concepts and demonstrates how user input and dynamic data structures can work together to create functional applications.
