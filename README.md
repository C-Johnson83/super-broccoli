# super-broccoli
Repository for module 19 challenge assignment: Progressive Web Application - Text Editor

## Description
The task involves creating a browser-based text editor for a single-page application that adheres to the criteria for Progressive Web Apps (PWAs). Additionally, the editor will incorporate multiple data persistence techniques to ensure redundancy in case a particular option is unsupported by the browser. Offline functionality is also a key feature.

To construct this text editor, begin with an existing application and implement methods for obtaining and storing data in an IndexedDB database. Utilize a package called idb, a lightweight wrapper around the IndexedDB API. This package, trusted by companies like Google and Mozilla, offers valuable methods for data storage and retrieval.

## Table of Contents
- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Installation and Usage](#installation-and-usage)
- [Features](#features)
- [License](#license)

## User Story
AS A developer  
I WANT to create notes or code snippets with or without an internet connection  
SO THAT I can reliably retrieve them for later use

## Acceptance Criteria
GIVEN a text editor web application
WHEN I open my application in my editor  
THEN I should see a client server folder structure  
WHEN I run `npm run start` from the root directory  
THEN I find that my application should start up the backend and serve the client  
WHEN I run the text editor application from my terminal  
THEN I find that my JavaScript files have been bundled using webpack  
WHEN I run my webpack plugins  
THEN I find that I have a generated HTML file, service worker, and a manifest file  
WHEN I use next-gen JavaScript in my application  
THEN I find that the text editor still functions in the browser without errors  
WHEN I open the text editor  
THEN I find that IndexedDB has immediately created a database storage  
WHEN I enter content and subsequently click off of the DOM window  
THEN I find that the content in the text editor has been saved with IndexedDB  
WHEN I reopen the text editor after closing it  
THEN I find that the content in the text editor has been retrieved from our IndexedDB  
WHEN I click on the Install button  
THEN I download my web application as an icon on my desktop  
WHEN I load my web application  
THEN I should have a registered service worker using workbox  
WHEN I register a service worker  
THEN I should have my static assets pre cached upon loading along with subsequent pages and static assets  
WHEN I deploy to Render  
THEN I should have proper build scripts for a webpack application

## Installation and Usage
Must have MongoDB and Node installed    
To install the super-broccoli, follow these steps:

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/C-Johnson83/super-broccoli.git
2. Change to the project directory:
    ```bash  
    cd super-broccoli  
3. Install the required dependencies using npm:  
    ```bash
    npm i  
4. Run the following command to start the app
    ```bash
    npm start   
5. Now you can view the app by going to  
    ```bash
    https://localhost:3000.com
 
## Features
- Offline Editing:
    
    Users can create and edit text content even when offline.
    Changes made offline are synchronized and saved to IndexedDB once the internet connection is restored.  

- Data Persistence:
 
    Utilizes IndexedDB for data storage, ensuring a reliable and efficient way to save and retrieve user content.
- Code Syntax Highlighting:
   
    Supports syntax highlighting for code snippets, enhancing the readability of programming content.
- Responsive Design:
   
    The text editor adapts to various screen sizes, providing a seamless user experience on both desktop and mobile devices.
- Service Worker Integration:
   
    Implements a service worker using Workbox to enable background sync, push notifications, and efficient caching of static assets.
- Install as Desktop App:
   
    Users can install the web application as a desktop app by clicking the Install button. The app icon will be added to the desktop for quick access.
- Webpack Bundling:
   
    Uses Webpack to bundle JavaScript files, ensuring efficient code organization and optimization.
- Next-gen JavaScript Support:
   
    The application is built using next-gen JavaScript features, ensuring compatibility with modern browsers while maintaining functionality.
- Client-Server Architecture:
   
    Features a client-server folder structure for clear separation of frontend and backend code.
- Render Deployment Scripts:
   
    Provides proper build scripts for deploying the application to Render, ensuring a smooth deployment process.

## License
This project is licensed under the MIT license.  
License Link  
https://opensource.org/licenses/MIT   
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]  