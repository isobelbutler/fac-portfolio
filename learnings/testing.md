## 1. Check that passing a given input into our tests returns the expected output

We have implemented several test cases using the `test` function, where we verify the behavior of functions based on specific inputs and check if they produce the expected results. For example, in the test called `test('Update list to be completed', () => {...})`, we simulate a user clicking on the completed icon, and then we use assertions to confirm that the task is marked as completed with the class `line-through`.

## 2. Write tests to mimic the behaviour of a user performing different actions

Throughout the test cases, we simulate user actions like clicking on buttons, filling out form fields, and interacting with completed or delete icons. For instance, in the test called `test('Passing test: Adding 1st task replaces the placeholder', () => {...})`, we mimic a user adding a new task by filling out the task title and description fields and then clicking the "Submit" button. We then assert that the added task replaces the placeholder task.

## 3. Write testable, modular functions

The code is structured with separate functions that handle specific tasks, making them easy to test individually. For example, the functions `addUserTask`, `openCreateTaskPopUp`, and `deleteTask` perform distinct actions, ensuring modular code that can be tested independently.

## 4. Write functions that add, remove or modify DOM nodes

The functions `renderTasksDOM`, `openCreateTaskPopUp`, `closeAddPopUp`, `addUserTask`, and `deleteTask` manipulate the DOM by adding, updating, or removing elements based on user interactions or data. These functions dynamically update the UI to reflect changes in tasks.

## 5. Apply event listeners to HTML form elements

Event listeners are applied to form elements like the "Submit" button and the "Add Task" button. For example, we use `addTaskForm.addEventListener('submit', ...)` to handle form submissions, and `addTaskBtn.addEventListener('click', ...)` to open the create task pop-up.

## 6. Use scope to control what variables are accessible inside functions and blocks

Our code appropriately scopes variables, preventing unintended conflicts and allowing functions to access the data they need. For instance, variables like `addTaskPop`, `userTaskTitle`, `userTaskDescription`, `taskItemHTML`, `taskContainer`, `toggleSwitch`, and `toggleMsg` are declared with proper scope to avoid ambiguity.

## 7. Use CSS grid to create complex layouts

Our CSS file includes various grid-related styles that allow us to create complex layouts for different sections of the website. For example, in the `#tasks-page` section, we use `display: grid` to organize the task list in a grid layout. The `toggle-container` uses `grid-template-columns: 1fr 1fr` to evenly distribute its child elements horizontally. By utilizing CSS grid, we can easily structure and align content on the page, making it more visually appealing and user-friendly.

## 8. Use CSS grid to make layouts that adapt to the viewport size

Our CSS file implements responsive design using CSS grid. For instance, in the media query `@media (min-width: 300px)`, we adjust the layout of the `.item-list` class by changing the `grid-template-columns` property to ensure that the task list adapts to different viewport sizes. Additionally, the `max-width` property is used in `#tasks-page` and `#item-list-container` to limit the width of these elements and allow them to resize based on the screen width. By incorporating CSS grid into our layout design, we ensure that the website content responds appropriately to various devices and screen sizes.
