
# Web-based Text Editor

Welcome to the Web-based Text Editor! This README provides you with a comprehensive guide to set up, run, and understand the core functionality of the application. This project consists of a text editor with client-server architecture, utilizing modern front-end technologies like Webpack, IndexedDB, and Service Workers.

## Table of Contents
1. [Folder Structure](#folder-structure)
2. [Installation](#installation)
3. [Running the Application](#running-the-application)
4. [Development Guide](#development-guide)
5. [Deploying to Render](#deploying-to-render)
6. [Application Features](#application-features)
7. [Contributing](#contributing)
8. [License](#license)



## Installation
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-repo/text-editor.git
   cd text-editor
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

## Running the Application
To start the application, run the following command from the root directory:
```bash
npm run start
```
This will launch the backend and serve the client-side application.

## Development Guide
### Webpack Bundling
The application uses Webpack to bundle JavaScript files and other assets. To bundle manually, you can run:
```bash
npm run build
```
This command will generate a bundled JavaScript file, a service worker, and a manifest file in the `client/public` directory.

### Using Modern JavaScript
The text editor supports next-gen JavaScript features thanks to Babel and other Webpack configurations. You should be able to write code using ES6+ without errors in the browser.

### IndexedDB Storage
The application uses IndexedDB for client-side data persistence. When you enter content in the text editor, it is saved to IndexedDB. This allows content retrieval after closing and reopening the application.

### Service Workers
Service workers are registered to enable offline functionality and asset caching. Upon loading, static assets are pre-cached using Workbox. You can also install the application as a Progressive Web App (PWA).

## Deploying to Render
To deploy this project to Render, ensure you have proper build scripts for a Webpack application. Render provides an automated build environment, and the following build commands are recommended:
```bash
# Set up environment variables if needed
# Run Webpack build script
npm run build
```
Ensure your backend server is correctly set up to serve the frontend's bundled files after deployment.

## Application Features
- **Text Editor**: A simple text editor with basic functionalities.
- **Offline Support**: Service workers and IndexedDB ensure offline functionality.
- **PWA Installation**: You can install the text editor as a Progressive Web App.
- **Modern JavaScript**: The application uses modern JavaScript features.
- **IndexedDB for Data Persistence**: Content is saved and retrieved from IndexedDB.

## Contributing
Contributions are welcome! If you would like to contribute to this project, please submit a pull request with your changes, and include a detailed explanation of your modifications.

