# conTextual
An offline-usable text editor.

## Overview

conTextual is an installable web text editor. You can install and use it offline to type to your heart's content. The editor will also save all your inputs. A handy little tool for all your notekeeping needs!

## Table of Contents



[Introduction]
[Folder Structure]
[Getting Started]
[Features]
[Deployment]
[Technologies Used]
[License]
Introduction
This is a text editor web application designed to provide a seamless editing experience with offline capabilities. The application utilizes modern web technologies such as Webpack, IndexedDB, and service workers to ensure efficient performance and reliability.

## Folder Structure
The project is organized into a client-server architecture:
```
root
├── client
│   ├── src
│   │   ├── js
│   │   ├── css
│   │   └── index.html
│   ├── webpack.config.js
│   └── package.json
├── server
│   ├── routes
│   ├── controllers
│   ├── models
│   └── server.js
├── package.json
└── README.md
```
client/: Contains all front-end related code.
server/: Contains all back-end related code.

## Getting Started
Prerequisites
Node.js
npm
## Installation
Clone the repository:


`git clone https://github.com/your-repo/text-editor.git`
`cd text-editor`

### Install dependencies:


`npm install`

## Running the Application
To start the application, run the following command from the root directory:

`npm run start`
This command will start up the backend server and serve the client application.


[Screenshot]("./images/Screenshot1.png")
## Features
Client-Server Architecture: Organized folder structure separating client and server code.
Bundling with Webpack: JavaScript files are bundled using Webpack.
Generated Assets: Webpack plugins generate an HTML file, service worker, and a manifest file.
Next-Gen JavaScript: The application supports and runs seamlessly with modern JavaScript features.
IndexedDB Integration: Automatically creates a database for storage when the editor is opened.
Auto-save Feature: Content is saved to IndexedDB when you click off the DOM window.
Persistent Storage: Retrieves content from IndexedDB when the editor is reopened.
PWA Installation: Allows downloading the web application as a desktop icon.
Service Worker: Registers a service worker using Workbox for offline capabilities.
Caching: Static assets and pages are pre-cached upon loading.

## Deployment
To deploy the application to Render, ensure you have proper build scripts for a Webpack application:

Set up the build scripts in package.json.
Configure your Render deployment settings to run the build and start commands.
## Technologies Used
Node.js: JavaScript runtime for server-side code.
Express: Web framework for Node.js.
Webpack: Module bundler for JavaScript.
IndexedDB: NoSQL database for client-side storage.
Workbox: Service worker libraries for offline caching.
## License

This project is licensed under the MIT License. See the LICENSE file for more details.

For any issues or contributions, please open a pull request or issue on the GitHub repository.