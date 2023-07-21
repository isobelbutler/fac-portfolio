## 1. Check that passing a given input into our tests returns the expected output

We have implemented several test cases using the test function, where we verify the behavior of functions based on specific inputs and check if they produce the expected results. For example, in the test called test('Update list to be completed', () => {...}), we simulate a user clicking on the completed icon, and then we use assertions to confirm that the task is marked as completed with the class line-through.

## 2. Write tests to mimic the behaviour of a user performing different actions

Throughout the test cases, we simulate user actions like clicking on buttons, filling out form fields, and interacting with completed or delete icons. For instance, in the test called test('Passing test: Adding 1st task replaces the placeholder', () => {...}), we mimic a user adding a new task by filling out the task title and description fields and then clicking the "Submit" button. We then assert that the added task replaces the placeholder task.

## 3. Write testable, modular functions

The code is structured with separate functions that handle specific tasks, making them easy to test individually. For example, the functions addUserTask, openCreateTaskPopUp, and deleteTask perform distinct actions, ensuring modular code that can be tested independently.

## 4. Write functions that add, remove or modify DOM nodes

The functions renderTasksDOM, openCreateTaskPopUp, closeAddPopUp, addUserTask, and deleteTask manipulate the DOM by adding, updating, or removing elements based on user interactions or data. These functions dynamically update the UI to reflect changes in tasks.

## 5. Apply event listeners to HTML form elements

Event listeners are applied to form elements like the "Submit" button and the "Add Task" button. For example, we use addTaskForm.addEventListener('submit', ...) to handle form submissions, and addTaskBtn.addEventListener('click', ...) to open the create task pop-up.

## 6. Use scope to control what variables are accessible inside functions and blocks

The code appropriately scopes variables, preventing unintended conflicts and allowing functions to access the data they need. For instance, variables like addTaskPop, userTaskTitle, userTaskDescription, taskItemHTML, taskContainer, toggleSwitch, and toggleMsg are declared with proper scope to avoid ambiguity.

## 7. Use CSS grid to create complex layouts

The provided HTML code includes CSS grid classes such as grid, flex, and center to organize and style elements in a structured grid layout. The layout structure helps to position and align elements consistently.

## 8. Use CSS grid to make layouts that adapt to the viewport size

By using CSS grid for layout design, the code allows the content to adapt and reflow based on different viewport sizes. Media queries can be applied to adjust column and row sizes or rearrange content, ensuring a responsive design that works well on various devices.
