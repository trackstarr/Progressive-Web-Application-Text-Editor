# Text Editor PWA

This is a text editor application that runs in the browser. It's a single-page application that meets the PWA (Progressive Web App) criteria and features a number of data persistence techniques that serve as redundancy in case one of the options is not supported by the browser. The application also functions offline.

## User Story

As a developer, I want to create notes or code snippets with or without an internet connection so that I can reliably retrieve them for later use.

## Features

- A client-server folder structure
- Starts up the backend and serves the client when `npm run start` is run from the root directory
- Bundles JavaScript files using webpack when the text editor application is run from the terminal
- Generates an HTML file, service worker, and a manifest file when webpack plugins are run
- Functions with next-gen JavaScript in the browser without errors
- Uses IndexedDB for immediate database storage creation and content saving
- Allows content retrieval from IndexedDB upon reopening the text editor
- Provides an Install button to download the web application as an icon on the desktop
- Registers a service worker using workbox upon loading the web application
- Caches static assets upon loading along with subsequent pages and static assets when a service worker is registered

## Installation

1. Clone the repository: `git clone https://github.com/yourusername/text-editor.git`
2. Navigate to the project directory: `cd text-editor`
3. Install dependencies: `npm install`
4. Start the application: `npm run start`

## Usage

1. Open the application in your browser.
2. You can start creating notes or code snippets.
3. The content will be saved to IndexedDB when you click off the DOM window.
4. The content will be retrieved from IndexedDB when you reopen the text editor.

## Deployment

1. Deploy to Heroku: `git push heroku main`
2. Ensure you have proper build scripts for a webpack application.

## Built With

- Webpack
- Babel
- IndexedDB
- Service Workers

## Contributing

Contributions are welcome. Please forward any contributions to peltierjames@gmail.com or contact me here on github

## License

This project is licensed under the MIT License
