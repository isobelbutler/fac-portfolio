## 1. Write code that executes asynchronously

We implemented asynchronous operations effectively in our code, particularly in the `fetchAPOD` and `fetchRandomSpaceImage` functions. By using asynchronous fetch requests, we ensured that the web page remained responsive during data retrieval from external APIs. For instance, when we submitted the form, our `handleFormSubmit` function used `fetchAPOD` to asynchronously fetch the Astronomy Picture of the Day from the NASA API.

## 2. Use callbacks to access values that aren’t available synchronously

Throughout our code, we skillfully employed callbacks to handle API responses. For example, in the `fetchAPOD` function, we used the `then` method to handle the response and extract the necessary data, such as the HD image URL and the description. Similarly, in `fetchRandomSpaceImage`, we utilized the `then` method to process the response and obtain the URL for a random space-related image.

## 3. Use promises to access values that aren’t available synchronously

Our code relied on promises, which played a crucial role in handling asynchronous operations. We applied promises effectively in functions like `fetchAPOD` and `fetchRandomSpaceImage`, leveraging the `fetch` API's promise-based structure to handle data retrieval and error handling gracefully.

## 4. Use the fetch method to make HTTP requests and receive responses

We made excellent use of the `fetch` method throughout our code to make HTTP requests to external APIs (NASA, Unsplash, and The Guardian) and receive their responses. For instance, in the `fetchAPOD` function, we used the `fetch` method to request data from the NASA API and retrieve the Astronomy Picture of the Day.

## 5. Configure the options argument of the fetch method to make GET and POST requests

While our code primarily focused on using the default GET method for API requests, we understood that the `fetch` method provides additional options to customize the behavior of requests, such as headers and request methods. Though our current code emphasized GET requests, we recognized the versatility of the `fetch` method to accommodate various request types.

## 6. Use the map array method to create a new array containing new values

## 7. Use the filter array method to create a new array with certain values removed

## 8. Access DOM nodes using a variety of selectors

We skillfully accessed DOM nodes using various selectors such as `getElementById`, `querySelector`, and `querySelectorAll`. This enabled us to target specific elements on the page and dynamically manipulate their content. For example, we used `querySelector` to obtain the form element and `getElementById` to access the date and headline elements.

## 9. Add and remove DOM nodes to change the content on the page

In our code, we effectively manipulated the DOM by updating the content of different elements. For instance, when fetching APOD or random space images, we changed the background image of the `apodDisplayElement` and updated the `apodDescriptionElement` to display relevant information.

## 10. Toggle the classes applied to DOM nodes to change their CSS properties

## 11. Use consistent layout and spacing

We followed a consistent layout and spacing guideline in our code, which contributed to readability and maintainability. By maintaining consistent spacing and alignment, we ensured that our codebase remained clean and easy to navigate.

## 12. Follow a spacing guideline to give our app a consistent feel

## 13. Debug client side JS in our web browser

Throughout development, we effectively used `console.log()` statements for debugging purposes. By logging relevant information and error messages to the browser console, we were able to diagnose and address issues efficiently.

## 14. Use console.log() to help us debug our code

We strategically placed `console.log()` statements in our code to provide helpful information during development. These logs offered valuable insights into the state of variables, function outputs, and errors, which greatly aided in debugging and refining the application.
