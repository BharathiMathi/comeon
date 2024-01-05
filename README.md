# Project Title - Comeon

This project is a responsive web application built with React and TypeScript.

## Technologies Used

- **React**: A JavaScript library for building user interfaces.
- **TypeScript**: A strict syntactical superset of JavaScript, adding optional static typing.

## Project Structure

This project is designed with a user-friendly interface and consists of several key components:

1. **Login Page**: The entry point of the application. Users are required to authenticate themselves to gain access to the application. The login page is designed to be simple and intuitive, ensuring a smooth user experience.

2. **Game List Page**: Upon successful login, users are directed to the Game List Page. This page displays a comprehensive list of available games. Each game is presented with relevant details for easy browsing. Additionally, a dynamic filtering feature is included on this page, allowing users to sift through the games based on the game category or game name, enhancing the navigation and search experience.

3. **Play Game Page**: When a user selects a game from the Game List Page, they are directed to the Play Game Page. This page is where the selected game can be played. It provides a seamless gaming experience within the application, ensuring users can enjoy their chosen games without navigating away from the application.

Overall, the project is structured to provide a seamless flow from login to game selection and gameplay, ensuring a user-friendly and engaging experience.

- **Organized Folder Structure**: The project follows a specific folder structure to make the codebase easier to navigate and maintain. Each feature of the application has its own directory, which contains all the related components and hooks functions. This modular structure promotes separation of concerns and makes it easier to find and update specific parts of the codebase, providing a better understanding of the functionality of each part of the application.

## Key Features

- **Semantic UI**: This project harnesses the power of Semantic UI, a development framework that focuses on a semantic approach to design. Semantic UI's human-friendly HTML has significantly enhanced the readability and maintainability of our codebase, ensuring that our interfaces are not only user-friendly but also developer-friendly..

- **Fetch API**: All REST API calls are made using the Fetch API, which is built into modern browsers. This avoids the need for additional dependencies for making HTTP requests.

- **Reusable Components, Hooks**: The project is structured to promote reusability, with common functionality extracted into reusable components and hooks.

- **Game Filtering Feature**: This project incorporates a dynamic game filtering feature that enhances user experience by allowing users to sift through games based on either the game category or game name. As users type in a game name or select a category, the list of displayed games adjusts in real-time to match the specified criteria. This intuitive feature facilitates a seamless browsing experience, making it quick and efficient to navigate through a large collection of games and find specific games of interest.

## Image Handling

In this project, images are conveniently placed within the `public` directory. This approach allows for straightforward referencing of these images throughout the application.

When the application receives an API response, it dynamically generates the appropriate image URLs. These URLs correspond to the image files located in the `public` directory. This strategy ensures that the correct images are displayed in the application based on the API response.

## State Management

- **Context API**: This project uses React's Context API for state management. The Context API provides a way to pass data through the component tree without having to pass props down manually at every level. This is particularly useful for sharing global data that many components need to access, such as user authentication information or theme settings. In this project, the Context API is used to share data between components, showcasing the ability to handle state in a more complex React application.

## Error Handling

- **Error Boundary**: This project uses Error Boundaries provided by React for better error handling. Error boundaries are React components that catch JavaScript errors anywhere in their child component tree, log those errors, and display a fallback UI instead of the component tree that crashed.

## Performance Optimization

- **React.lazy**: This project uses `React.lazy` for code splitting by route. `React.lazy` function lets you render a dynamic import as a regular component. It helps to load components lazily as they are rendered, which can significantly improve performance in larger apps.

- **Loading Component**: A loading spinner is displayed while components are being lazily loaded. This provides a better user experience by giving visual feedback during potentially long loading times.

## Testing

Unit testing is currently not implemented in this project, but it's a key enhancement planned for future updates. The intention is to use Jest for creating unit tests and React Testing Library for testing React components, to ensure code reliability and correctness.

## Running the Project Locally

To run the project locally:

1. Clone the repository to your local machine.
2. Navigate to the project directory in the terminal.
3. Run `npm install` to install the project dependencies.
4. Run `npm start` to start the frontend development server.
5. Run `npm install -g json-server` and `json-server --watch src/mock/mock-data.json --port 3001    --middlewares src/mock/mock-api.js`to start the backend development server.
