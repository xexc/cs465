# cs465
Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page application (SPA).

A section of the site used Express, HTML, and JavaScript to display web pages. By leveraging Express and JavaScript, routes and controllers were created to manage browser requests for specific pages. Express would then either serve a static HTML page or generate a dynamic page using Handlebars templates filled with data from the database. These tools worked together to manage server requests and deliver the results to the frontend client. The Angular portion of the project functioned differently: upon the first page load, the entire single-page application (SPA) is sent to the client. From that point on, all page rendering and code execution happen client-side within the browser. Backend calls are only necessary for retrieving data from the database. With Express, each page load or refresh triggers multiple server calls. In contrast, an SPA takes longer to load initially as it fetches all the necessary code from the backend at once. However, after that first load, no additional server calls are needed for navigating within the SPA.


Why did the backend use a NoSQL MongoDB database?

MongoDB offers strong scalability and fast querying capabilities. Its document structure is compatible with JSON formatting, making it an excellent fit for integration with frontend applications.


How is JSON different from Javascript and how does JSON tie together the frontend and backend development pieces?

JSON (JavaScript Object Notation) is a data format, whereas JavaScript is a programming language. JSON is primarily used for structuring data in a way that is both easy to read and parse, while JavaScript is a full-fledged language capable of handling logic, operations, functions, and more.


Provide instances in the full stack process when you refactored code to improve functionality and efficiencies, and name the benefits that come from reusable user interface (UI) components.

An example of enhancing functionality through refactoring was the replacement of static HTML pages with Handlebars templates. This approach allowed for the reuse of page structure while enabling dynamic content display. Another improvement involved moving the data used to populate templates from static JSON files within the codebase to MongoDB. This shift allows for content updates or changes without needing to redeploy or modify the website’s code.


Methods for request and retrieval necessitate various types of API testing of endpoints, in addition to the difficulties of testing with added layers of security. Explain your understanding of methods, endpoints, and security in a full stack application.

HTTP methods define different ways a client can interact with a server. Common HTTP methods include GET, POST, PUT, and DELETE. These methods enable the client to communicate with the server via API endpoints. Security for this full-stack application involved authenticating users and providing them with a valid JWT, allowing them access to certain endpoints.


