1. **Find the difference between a traditional webpage and a single-page application (SPA).** Hint: (read [paragraph](https://learn.microsoft.com/en-us/dotnet/architecture/modern-web-apps-azure/modern-web-applications-characteristics#traditional-and-spa-behaviors-supported)) <br>

   **Traditional Web Applications:** <br>
   Traditional web applications are slower and less efficient because they rely heavily on the server. Every time content on the page needs to change, the browser must send a new request to the server, reload the page, and fetch the updated content. This frequent page reloading leads to delays and reduced responsiveness.

   **Single-Page Applications (SPAs):** <br>
   Single-page applications, on the other hand, load most of their HTML, JavaScript, and CSS files during the initial page load. Instead of relying on full page reloads, SPAs handle most updates dynamically on the client side, which improves responsiveness and creates a smoother user experience. While SPAs still communicate with the server to fetch or send data, they typically use asynchronous requests (e.g., via AJAX or APIs) to minimize disruptions and keep the application running seamlessly.

2. **Explain the difference between a Web App and a Web API.**
   **Web Application:**<br>
   A web application is a complete software application that runs in a web browser. It typically includes a graphical user interface (GUI) built with HTML, CSS, and JavaScript to allow user interaction. A web app may also have functionality that involves making requests to a server to fetch or send data, such as logging in or retrieving information from a database. The web app is run on the client side (in the browser).

   **Web API:**<br>
   A web API (Application Programming Interface) is a server-side application that provides endpoints to perform specific tasks, such as fetching data from a database, processing requests, or managing authentication. It does not have a user interface and is often used by web applications to communicate with the server. For example, a web API might retrieve product details from a database and return the data to the web app for display.

   **Key Difference:**<br>
   While a web application is run on the client side and interacts with users directly, a web API is implemented and runs on the server. A web API is usually accessed programmatically by the web app or other clients (such as mobile apps) to enable specific functionality.

3. **Explain the difference between back-end and front-end**
   Back-end also called the server is the brains of a web-application. The back-end is typically a big cluster of computers in a datacenter that runs the program wich the front-end can communicat with. The front-end is typically an interface run on the client computer, typically built using HTML, CSS, and JavaScript. The front-end is responsible for displaying content, handling user input, and providing an intuitive experience. While the front-end does some processing (e.g., form validation or animations), it primarily depends on the back-end for data and functionality. Common back-end technologies include programming languages like Python, Java, or Node.js, and databases like MySQL, MongoDB.

4. **Write in your own words what each of the following terms means in the context of Web APIs development:**

   - **Middleware** <br>
     In the context of Web APIs, middleware is software that sits between the front-end and back-end. It intercepts incoming HTTP requests before they reach the back-end and can perform tasks such as authentication, logging, or data validation. Middleware is often used in frameworks like Express.js to manage the request/response cycle and add functionality to an application.

   - **Endpoint** <br>
     An endpoint is a specific URL within an API that a client can use to interact with the back-end. It represents a resource or functionality that the API exposes. For example, an endpoint like /users/123 could be used to fetch data about a specific user. Endpoints typically define the operations a client can perform, such as GET, POST, PUT, or DELETE.

   - **Route** <br>
     A route refers to a specific path in the URL structure of a web application or API. In the context of APIs, a route maps a URL to a particular function or controller that handles the request. For example, in /products/list, /products is the base route, and /list specifies a nested route. Routes often determine how the application responds to HTTP requests.

   - **Controller** <br>
     A controller is a component in the back-end, particularly in Model-View-Controller (MVC) architecture. It defines and manages the logic for specific routes or endpoints. Controllers handle incoming requests, interact with the model to fetch or modify data, and send appropriate responses back to the client. For example, in a .NET or Node.js application, a controller may define the methods for endpoints like GET /users or POST /orders.

   - **Dependency Injection** <br>
     Dependency injection (DI) is a design pattern where a framework or library provides the necessary dependencies (such as services or objects) to a component rather than the component creating them itself. This makes the code more modular and easier to test. For example, in frameworks like Spring (Java) or .NET, you can use DI to inject a database service or configuration object into your controllers or middleware without manually instantiating them.
   - Hint: [ASP.NET Core fundamentals overview](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/?view=aspnetcore-8.0&tabs=linux)
