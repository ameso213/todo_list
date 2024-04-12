The Todo List is contained within a <div> element with the class container.
It consists of a "Todo List" as the heading, an <input> field for entering tasks, an "Add Task" <button>, and a <ul> element with the id taskList where tasks will be displayed.
JavaScript Functionality:
It consists three functions;
the addTask, the deleteTask and the updateTask which can add a task , update it and delete it as well
i used the buttons 


The addTask() function is called when the "Add Task" button is clicked. It gets the value of the task input field, trims any leading or trailing 
whitespace, and adds the task to the tasks object if it's not empty. Then it calls displayTasks() to update the display.

The updateTask(task) function is called when the user wants to update the description of a task. It prompts the user to enter a new description,
updates the description in the tasks object, and then calls displayTasks() to reflect the changes.

The deleteTask(task) function is called when the user wants to delete a task. It confirms with the user if they're sure about deleting the task,
then removes the task from the tasks object and calls displayTasks() to update the display.

The displayTasks()function updates the display of tasks in the <ul> element. It first clears the existing list, then iterates over the tasks object, 
creating a <li> element for each task. It displays the task name and its description (if available), along with "Edit" and "Delete" buttons.
These buttons use Font Awesome icons for better user experience.
The displayTasks() function is called initially to display any existing tasks in the tasks object when the page loads.
