<p align="center">
  <img src="https://github.com/glenntanjoh/CodeSLime/blob/61d739a691be313eaf8731ac627f916fbef2ea5a/logo.png?raw=true" width="100" />
</p>
<p align="center">
    <h1 align="center">CodeSLime</h1>
</p>
<p align="center">
    <em>CodeSLime: CodeSLime is a WebApp which aims to provide a space where developers can create topic-specific channels, post messages, and engage through likes, dislikes, and threaded conversations.</em>
</p>
<p align="center">
	<img src="https://img.shields.io/github/license/glenntanjoh/CodeSlime?style=default&color=0080ff" alt="license">
	<img src="https://img.shields.io/github/last-commit/glenntanjoh/CodeSlime?style=default&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/glenntanjoh/CodeSlime?style=default&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/glenntanjoh/CodeSlime?style=default&color=0080ff" alt="repo-language-count">
<p>
<p align="center">
	<!-- default option, no dependency badges. -->
</p>
<hr>

## Quick Links

- [Overview](#overview)
- [Features](#features)
- [Repository Structure](#repository-structure)
- [Modules](#modules)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Running CodeSlime](#running-codeslime)

---

## Overview


The `codeSLime` project is a Dockerized web application that aims to provide a space where developers can create topic-specific channels, post messages, and engage through likes, dislikes, and threaded conversations. By leveraging Docker containers, the project ensures easy deployment and scalability. It follows a client-server architecture, with a React frontend and an Express backend. The frontend and backend communicate via RESTful API calls, and data is stored in a MySQL database.

---

##  Features

|    |   Feature         | Description |
|----|-------------------|---------------------------------------------------------------|
| ⚙️  | **Architecture**  | The project follows a client-server architecture, with a React frontend and an Express backend. It uses a MySQL database for data storage. The frontend and backend communicate via RESTful API calls. |
| 🔩 | **Code Quality**  | The codebase emphasizes clean and modular code. It follows best practices and adheres to a consistent coding style. Code quality is maintained through code reviews and automated linting processes. |
| 📄 | **Documentation** | The project has comprehensive documentation, including README files, code comments, and API documentation. It provides clear instructions on how to set up and run the project. |
| 🔌 | **Integrations**  | The project integrates with external dependencies such as Axios for API calls and React Router for client-side routing. It also includes integrations with libraries like lodash.debounce and aos for additional functionality. Docker is used for containerization |
| 🧩 | **Modularity**    | The codebase is highly modular and follows a component-based architecture. Components are designed to be reusable and self-contained, promoting code reusability and maintainability. |
| 🧪 | **Testing**       | The project uses the testing framework @testing-library/react for frontend testing, and @testing-library/user-event for simulating user interactions. It also includes server-side testing using express-async-handler. |
| ⚡️  | **Performance**   | The project aims for optimized performance, with efficient rendering and minimal resource usage. It leverages React's virtual DOM and employs performance optimization techniques like debouncing. |
| 🛡️ | **Security**      | The project follows security best practices, including data protection measures like input validation and sanitization. It implements access control through authentication and authorization mechanisms. Data protection accomplished via 'bcryptjs' for hashing passwords. Also, uses 'express-session' for session management. |
| 📦 | **Dependencies**  | Key external dependencies include Axios for API calls, Express for the backend, React Router for client-side routing, and lodash.debounce for debouncing. |

---

##  Repository Structure

```sh
└── CodeSlime/
    ├── codeslime
    │   ├── package-lock.json
    │   ├── package.json
    │   ├── public
    │   │   ├── index.html
    │   │   ├── manifest.json
    │   │   └── robots.txt
    │   └── src
    │       ├── App.js
    │       ├── App.test.js
    │       ├── components
    │       ├── context
    │       ├── index.css
    │       ├── index.js
    │       ├── pages
    │       ├── reportWebVitals.js
    │       ├── setupTests.js
    │       └── styles
    ├── docker-compose.yml
    ├── Dockerfile
    ├── package-lock.json
    ├── package.json
    ├── server.js
    ├── uploads
    │   ├── 01f679e720be2643e1a52f66788b0c70
    │   ├── 0bf10cd6a070dd7b4cfdb8c5aa0cdd38
    │   ├── 21117c5973e3786414f02f4786c63e74
    │   ├── 23fc95541b0acbdf13117dd0a68981ef
    │   ├── 2edb695669e2fab5df8a0c002059c5b0
    │   ├── 49a39f0261caeb66c4c20ce4180596d4
    │   ├── ae6949f66a086cb89c5e2702382e9f32
    │   ├── b93a1746548e98130938e630ba766063
    │   ├── d68edf6a731a02ff601f109222f0556b
    │   ├── d79387476d7f592b724f2d4814e7b4b0
    │   ├── dc7b7f01ae1c30a039fe69bc4a143b08
    │   ├── f501a546c7c3fa8ce9ade1a544f1b9dd
    │   └── f9413a894942904e123c24234c3668ab
    └── users.txt
```

---

##  Modules

<details closed><summary>.</summary>

| File                                                                                             | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ---                                                                                              | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [.gitignore](https://github.com/glenntanjoh/CodeSlime/blob/master/.gitignore)                 | The provided .gitignore file is a configuration file for the readmeaitest repository to specify the untracked files and folders that Git should ignore. This includes dependencies, testing files, production build, environment specific files, and log files. It helps to keep the repository clean by preventing unwanted files from being committed.                                                                                                                                                                        |
| [docker-compose.yml](https://github.com/glenntanjoh/CodeSlime/blob/master/docker-compose.yml) | The code snippet in the `docker-compose.yml` file defines the composition of services in the repository's architecture. Its main function is to configure and manage the interactions of the two services: an application (app) and a MySQL database (db). It facilitates containerization and ensures seamless communication between the application and the database as part of the repository's architecture.                                                                                                                                                                                    |
| [Dockerfile](https://github.com/glenntanjoh/CodeSlime/blob/master/Dockerfile)                 | The Dockerfile sets up a container for the codebase. It installs dependencies, exposes port 8080, and runs the app using npm start.                                                                                                                                                                                                                                                                                                                                                                                                   |
| [package-lock.json](https://github.com/glenntanjoh/CodeSlime/blob/master/package-lock.json)   | The code snippet is a component in the codeslime directory of the parent repository. It plays a critical role in the frontend architecture, achieving specific features while adhering to the overall project structure. Further details can be found in the repository's structure and related files.                                                                                                                                                                                                                                |
| [package.json](https://github.com/glenntanjoh/CodeSlime/blob/master/package.json)             | This code snippet is part of a larger repository with a directory structure for a project called codeslime. The code is contained within the `package.json` file and defines the dependencies required by the project. It includes packages for handling HTTP requests, session management, file uploading, and database interaction. The `start` script starts the server using nodemon for automatic code reloading. Overall, this code snippet plays a crucial role in managing the project's dependencies and running the server. |
| [server.js](https://github.com/glenntanjoh/CodeSlime/blob/master/server.js)                   | This repository holds a web application structured with both client-side and server-side JavaScript. The main code resides in the codeslime directory and includes App.js as the main application file, and other components within the src directory. The server.js file at the repository root handles server-side tasks. The uploads folder stores user-generated content.                                                                                                                                                                                                                                         |
| [users.txt](https://github.com/glenntanjoh/CodeSlime/blob/master/users.txt)                   | The users.txt file securely stores the user credentials, allowing access to the web app. This contains credentials you can use to test the app functionalities.                                                                                                                                                                                                                                                                                                                                        |

</details>

<details closed><summary>codeslime</summary>

| File                                                                                                     | Summary                                                                                                                                                                                                                                                                                                                                             |
| ---                                                                                                      | ---                                                                                                                                                                                                                                                                                                                                                 |
| [package-lock.json](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\package-lock.json) | This code snippet is part of a larger repository called CodeSlime. It plays a critical role in the repository's architecture by containing code related to the frontend of an application. It includes files for components, context, and styling, among others. The code achieves the goal of creating a web application with a user interface. |
| [package.json](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\package.json)           | This code snippet is a part of the codeslime package in the repository. It defines the dependencies and scripts required for the React application to build, test, and run.                                                                                                                                                                         |

</details>

<details closed><summary>codeslime.public</summary>

| File                                                                                                    | Summary                                                                                                                                                                                                                                                                                                             |
| ---                                                                                                     | ---                                                                                                                                                                                                                                                                                                                 |
| [index.html](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\public\index.html)       | The code snippet in the `index.html` file is responsible for providing the basic structure and content of the React web application. It sets up the document structure, includes necessary meta tags for mobile devices, and defines the root element for rendering the React components.                           |
| [manifest.json](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\public\manifest.json) | This code snippet is responsible for defining the manifest.json file for a React app. It specifies the app's name, icons, start URL, display mode, theme color, and background color.                                                                                                                               |
| [robots.txt](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\public\robots.txt)       | The code snippet in `codeslime/public/robots.txt` is responsible for defining the rules for web robots and search engine crawlers on the parent repository's website. It follows the standards set by `https://www.robotstxt.org/robotstxt.html` and allows access to all parts of the website for all user agents. |

</details>

<details closed><summary>codeslime.src</summary>

| File                                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                   |
| ---                                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                       |
| [App.js](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\App.js)                         | The `App.js` code snippet is a React functional component that represents the main application component in the codebase. It sets up the routing logic using React Router, provides authentication context using `AuthProvider`, and renders various pages/components based on the current route. It also includes state management for the visibility of a channel form. |
| [App.test.js](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\App.test.js)               | The `App.test.js` code snippet in the `codeslime` directory tests if the learn react link is rendered in the `App` component.                                                                                                                                                                                                                                             |
| [index.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\index.css)                   | This code snippet in the index.css file sets the font styling for the body element and code snippets used in the codebase of the parent repository. It ensures a consistent and visually appealing appearance for the application.                                                                                                                                        |
| [index.js](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\index.js)                     | This code snippet is the entry point for a React application. It renders the main component, `App`, in strict mode. It also includes a function, `reportWebVitals`, to measure performance.                                                                                                                                                                               |
| [reportWebVitals.js](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\reportWebVitals.js) | The `reportWebVitals.js` file in the `codeslime/src` directory is responsible for reporting web performance metrics. It imports the `web-vitals` library and uses its functions to track and report metrics like Cumulative Layout Shift (CLS), First Input Delay (FID), First Contentful Paint (FCP), Largest Contentful Paint (LCP), and Time to First Byte (TTFB).     |
| [setupTests.js](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\setupTests.js)           | The code snippet in setupTests.js adds custom Jest matchers for asserting on DOM nodes. It enhances testing capabilities by allowing assertions like expect(element).toHaveTextContent(/react/i). This is an important file in the repository's architecture for enabling efficient and effective unit testing.                                                           |

</details>

<details closed><summary>codeslime.src.components</summary>

| File                                                                                                                | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ---                                                                                                                 | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| [AdminPanel.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\AdminPanel.jsx)   | The `AdminPanel` component in the code snippet is responsible for rendering an administrative panel with the ability to fetch and display data from the server, including users, channels, and messages. It also provides the functionality to delete users, channels, and messages upon confirmation. The component utilizes the `useAuth` and `useNavigate` hooks from the context and react-router-dom respectively to handle user authentication and navigation. |
| [ChannelCard.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\ChannelCard.jsx) | This code snippet is a React component called ChannelCard. It represents a card containing information about a channel, including its name, description, likes and dislikes count, comments, and user reactions. Users can view and post comments, as well as like or dislike the channel. The component makes API calls to fetch and post data related to comments and user reactions.                                                                              |
| [ChannelForm.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\ChannelForm.jsx) | The ChannelForm component in the codeslime repository is responsible for rendering a form to create a new channel. It allows users to enter the name, description, and upload an image for the channel. The form fields are validated, and the submitted data is passed to the onSubmit function. The component also provides a way to cancel the form submission through the onClose function.                                                                      |
| [Comments.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\Comments.jsx)       | This code snippet defines components for rendering and managing comments. It allows users to reply to comments and displays the comment thread. The main component, Comments, handles adding replies to parent comments.                                                                                                                                                                                                                                             |
| [ImageUpload.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\ImageUpload.jsx) | This code snippet is a React component called ImageUpload. It allows users to select and upload an image file. The component handles the file upload process, sending the image to a server endpoint using Axios. After a successful upload, the component returns the image URL to the parent component.                                                                                                                                                            |
| [LandingPage.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\LandingPage.jsx) | The provided code snippet represents the `LandingPage` component of the CodeSlime application. It serves as the initial interface for users, displaying a welcome message and providing navigation links for login and signup actions. Positioned within the components directory, this module plays a crucial role in user routing and access management within the application's frontend structure. Router.                                                                                                                                                                                                                                                                              |
| [LoginForm.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\LoginForm.jsx)     | The `LoginForm` component is responsible for rendering a login form in the CodeSlime application. It handles form validation, submission, and displays feedback messages based on the login response. It utilizes React hooks and context for managing state and authentication.                                                                                                                                                                                     |
| [Navbar.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\Navbar.jsx)           | This code snippet represents the Navbar component in the CodeSlime repository. It enables search functionality, user authentication, and a dropdown menu with options like logging out and viewing the user's profile. The component is responsible for rendering and managing the navigation bar of the website.                                                                                                                                                    |
| [SignupForm.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\components\SignupForm.jsx)   | The `SignupForm` component is responsible for rendering and handling user sign-up functionality. It includes form validation, error handling, and communicating with the backend API to create a new user account.                                                                                                                                                                                                                                                   |

</details>

<details closed><summary>codeslime.src.context</summary>

| File                                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                                   |
| ---                                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                                       |
| [AuthContext.js](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\context\AuthContext.js) | The `AuthContext.js` code snippet is part of the `codeslime` directory in the repository. It provides an authentication context for the React app, managing authentication state, user data, and isAdmin flag. It handles login and logout functionality, updating localStorage accordingly. Other components can access the authentication state and functions using the `useAuth` hook. |

</details>

<details closed><summary>codeslime.src.pages</summary>

| File                                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                              |
| ---                                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                                  |
| [HomePage.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\pages\HomePage.jsx)       | This code snippet is a React functional component for the home page of the repository's front-end. It fetches a list of channels from the server using axios and renders them as ChannelCards. It also provides a form to create new channels.                                                                                                                                       |
| [LandingPage.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\pages\LandingPage.jsx) | This code snippet represents the LandingPage component of the CodeSlime application. It renders a landing page with a hero section and features section. Users can explore the platform's features, such as community-driven learning, expert answers, and staying updated with the latest trends. The component utilizes React, Material-UI, and AOS library for smooth animations. |
| [LoginPage.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\pages\LoginPage.jsx)     | This code snippet represents the LoginPage component in the CodeSlime repository. It renders a login page with a title and a login form. It is responsible for presenting the login functionality to the user.                                                                                                                                                                       |
| [SignupPage.jsx](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\pages\SignupPage.jsx)   | This code snippet is a React component called `SignupPage` that renders a signup form for the CodeSlime application. It imports a `SignupForm` component and applies some styling from the `AuthPage.css` file. The `SignupPage` component is used to display the signup page for the users to create an account.                                                                    |

</details>

<details closed><summary>codeslime.src.styles</summary>

| File                                                                                                            | Summary                                                                                                                                                                                                                                                                                           |
| ---                                                                                                             | ---                                                                                                                                                                                                                                                                                               |
| [App.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\App.css)                 | The code snippet, located in `codeslime/src/styles/App.css`, defines the styling for the main App component of the project. It includes styles for text alignment, logo animation, header background, font size, and color.                                                                       |
| [AuthForm.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\AuthForm.css)       | The code snippet at `codeslime/src/styles/AuthForm.css` defines the styling rules for an authentication form. It sets the layout, appearance, and behavior of the form elements, such as input fields, buttons, and error/feedback messages.                                                      |
| [AuthPage.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\AuthPage.css)       | The AuthPage.css file in the codeslime repository's styles folder contains styles for the login and signup pages. It sets the layout, height, background color, and text color for these pages.                                                                                                   |
| [ChannelCard.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\ChannelCard.css) | The ChannelCard.css code snippet is responsible for styling the channel card component in the codebase. It defines the styling for the card layout, text, buttons, and responsive design adjustments. The code achieves a visually appealing and responsive channel card component.               |
| [ChannelForm.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\ChannelForm.css) | The code snippet in ChannelForm.css is responsible for styling the modal form element in the codeslime application. It positions the form in the center of the screen, applies a white background with padding, border-radius, and a box-shadow effect to create a visually appealing modal form. |
| [Comments.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\Comments.css)       | The code snippet in `Comments.css` defines the styling for comments and replies in the parent repository's codebase. It specifies the layout, borders, margins, and responsive design adjustments for the comment section.                                                                        |
| [HomePage.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\HomePage.css)       | The code snippet in the `HomePage.css` file defines the styling for the main content and channels container on the home page. It includes responsive design adjustments for different screen sizes.                                                                                               |
| [LandingPage.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\LandingPage.css) | The code snippet located at `codeslime/src/styles/LandingPage.css` contains the CSS styling for the landing page of the codebase. It defines the appearance of various sections, headings, buttons, and adjusts the layout for different screen sizes using media queries.                        |
| [Navbar.css](https://github.com/glenntanjoh/CodeSlime/blob/master/codeslime\src\styles\Navbar.css)           | The code snippet is a CSS file, `Navbar.css`, that defines the styling for the navigation bar component. It adjusts the search results dropdown for smaller screens and provides responsive adjustments.                                                                                          |

</details>

---

##  Getting Started

***Requirements***

Ensure you have the following dependencies installed on your system:

* **JavaScript**: `version x.y.z`

###  Installation

1. Clone the CodeSlime repository:

```sh
git clone https://github.com/glenntanjoh/CodeSlime
```

2. Change to the project directory:

```sh
cd CodeSlime
```

3. Install the dependencies:

```sh
npm install
```

###  Running CodeSlime

This has to be done using two terminals. In the first terminal;

Use the following command to run the backend:

```sh
npm start
```

Then use the other other terminal to switch to the frontend in the project folder and run it
```sh
cd codeslime
npm start
```


