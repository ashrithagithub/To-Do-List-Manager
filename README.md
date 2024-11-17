# To-Do-List-Manager

Create a simple console application to manage a list of tasks. Users can add, remove, and view their tasks.






#Project Breakdown:

• Task Input (Reference 2): Use console input to let users add and remove
tasks.

• Display Task List: Show all tasks in a clear and organized format.

• Data Storage: Store tasks in an array or list and provide options for adding
and removing tasks.

• Outcome: A functional to-do list application that manages tasks using basic
user input and array operations.







#Description of To-Do List Manager Program

This Java program, named ToDoListManager, is a console-based application designed to help users efficiently manage a to-do list. It enables users to add tasks, view all tasks, and remove tasks from their list. The program uses a simple text-based menu system and makes use of Java's ArrayList and Scanner classes for dynamic task management and user input handling, respectively. This project is perfect for beginners who want to learn about Java collections, loops, and switch-case constructs.






#Working Procedure (Detailed Explanation):

The ToDoListManager program is broken down into several functionalities, each corresponding to a menu option presented to the user. Here’s a step-by-step explanation of how the program works:

________________________________________
1. Initial Setup and Variables
   
•	The program begins by importing essential Java utilities:

• ArrayList is used to store the tasks dynamically.

•	Scanner is used to accept user input.

•	An ArrayList named tasks is initialized to hold the list of tasks.

•	The variable choice is used to store the user's menu selection.

________________________________________
2. Main Menu and User Input Loop
   
•	The program uses a do-while loop to continuously prompt the user for actions until they choose to exit.

•	The menu options displayed are:

1.	Add a task
2.	View all tasks
3.	Remove a task
4.	Exit the application
•	The user is prompted to enter their choice, which is stored in the choice variable.
________________________________________
3. Adding a Task
•	When the user selects option 1:
•	The program prompts the user to enter a task description.
•	The entered task is added to the tasks list using the add() method.
•	A confirmation message, "Task added!", is displayed.

Example:
Enter task: Complete Java assignment
Task added!
________________________________________
4. Viewing All Tasks
•	When the user selects option 2:
•	If the tasks list is empty, the program displays "No tasks to display!".
•	If there are tasks present, the program iterates through the list and displays each task with a corresponding number.


Example Output:

Your Tasks:
1. Complete Java assignment
2. Review notes for the exam
________________________________________
5. Removing a Task
•	When the user selects option 3:
o	If the tasks list is empty, the program displays "No tasks to remove!".
o	If tasks exist, the program displays all tasks with their corresponding numbers.
o	The user is prompted to enter the task number they wish to remove.
o	The program checks if the entered number is valid:
	If valid, it removes the selected task using the remove() method.
	If invalid, it displays "Invalid task number!".


Example:

Your Tasks:
1. Complete Java assignment
2. Review notes for the exam
Enter task number to remove: 1
Task removed!
________________________________________
6. Exiting the Application
•	When the user selects option 4:
o	The program exits the loop and displays "Exiting... Goodbye!".
•	The scanner.close() method is called to release system resources.


Example:

Exiting... Goodbye!

________________________________________
7. Handling Invalid Inputs
•	If the user enters an invalid option (i.e., anything other than 1, 2, 3, or 4), the program displays an error message:

Invalid choice! Please try again.
•	The program then returns to the main menu, allowing the user to try again.
________________________________________
Summary of Key Concepts Used

•	ArrayList: This data structure is used because of its dynamic size, allowing tasks to be added and removed easily.
•	Scanner: The program uses Scanner for reading user inputs from the console.
•	Loops (do-while): Ensures the menu is displayed repeatedly until the user chooses to exit.
•	Conditional Statements (switch-case): Efficiently handles different user choices.
•	Exception Handling: Although not explicitly used in this code, user input validation prevents some common errors.

________________________________________
This simple yet powerful program demonstrates the fundamentals of Java programming while providing a practical tool that can be extended in the future with features like saving tasks to a file, editing tasks, setting deadlines, or even adding a graphical user interface (GUI).



