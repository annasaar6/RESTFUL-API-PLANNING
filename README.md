# RESTFUL-API-PLANNING

Documentation | Art Institute of Chicago API
Repository: https://github.com/annasaar6/RESTFUL-API-PLANNING


Step 1: API Selection
The selected public API is the Art Institute of Chicago API. This API provides access to artwork information, artist details, collections, and museum resources. It is suitable for this assignment because it is publicly available, well documented, and returns structured JSON data that can be processed easily in a web application. The purpose of the application is to allow users to search for and explore artwork information through a simple interface.


Step 2: REST Principles
The application design follows REST principles. Resource identification is achieved through unique artwork endpoints. Statelessness means every request contains the information required for processing and does not depend on previous requests. Standard HTTP methods provide consistent communication between the application and the API. These principles support interoperability, scalability, and maintainability.


Step 3: Endpoint Mapping
The application will use the GET /api/v1/artworks endpoint to retrieve collections of artwork records. The GET /api/v1/artworks/{id} endpoint will retrieve detailed information about a specific artwork. The GET /api/v1/artworks/search?q=keyword endpoint will return search results that match user-entered keywords. These endpoints return JSON data that will be displayed within the user interface. A future Flask backend could include a POST endpoint that accepts JSON search activity data and returns confirmation messages.


Step 4: Data Flow Diagram (Textual)
The user opens the application and enters a search term. A loading indicator appears while the request is processed. The application sends a request to the Art Institute of Chicago API. The API returns JSON data. The application validates and processes the response, checks for errors, and renders the resulting artwork information in the user interface. If an error occurs, a user-friendly message is displayed. Users can then submit additional searches.


Step 5: Fetch API Usage
The Fetch API will be used to perform asynchronous GET requests. Request headers may be included when necessary to identify the expected response format. Because requests are asynchronous, the user interface remains responsive while data is retrieved. Successful responses are converted from JSON into JavaScript objects. Failed requests display clear error messages while loading indicators communicate system activity to the user.


Step 6: Dynamic Rendering and Conditional Styling
JSON data returned by the API will be mapped to artwork cards or list-style displays. Artwork titles, artist names, dates, and departments will be displayed dynamically. Conditional styling will be applied based on specific data values. Public-domain artworks may display a highlighted badge, while records without image resources may use a neutral visual style. These distinctions help users quickly identify important information.


Step 7: Form Handling
The application will include a keyword search field, maximum results field, and search button. User-entered information will be collected after validation and placed into a JavaScript object. The information will then be transformed into JSON format. This JSON payload could be submitted to a future Python Flask backend for analytics, activity logging, or reporting purposes.


Step 8: Form Controls and Validation
The keyword search field is required and must contain at least one character. The maximum results field must contain a positive number within an acceptable range. Validation messages will notify users when required information is missing or incorrectly entered. After validation is complete, the application will create a JSON payload containing the keyword, result limit, and timestamp before submission to a future backend service.


Step 9: Technology Stack
HTML5 will provide page structure, CSS3 will provide styling, JavaScript will provide application logic, and the Fetch API will retrieve data from the Art Institute of Chicago API. Git and GitHub will support version control and repository management. Browser Developer Tools will be used for testing, debugging, and inspecting API responses. Flask is identified as a future backend technology.


Step 10: Implementation Steps
The project will begin with repository creation and review of the API documentation. Next, Fetch GET requests will be implemented together with loading and error states. Artwork results will then be rendered dynamically within the interface. Form controls and validation rules will be added, followed by conditional styling enhancements. Finally, testing, documentation review, repository cleanup, and submission preparation will be completed.
