# Electron + Tailwind CSS Template

This is a basic Electron app template using Tailwind CSS, created by SK-Digital. It provides a simple and efficient starting point for your Electron projects.

## Features

- Electron for cross-platform desktop apps
- Tailwind CSS for rapid UI development
- Modern, clean UI with a dark theme
- Basic project structure and configuration

## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed the latest version of [Node.js and npm](https://nodejs.org/)
- You have a basic understanding of JavaScript and Electron

## Installing Electron + Tailwind CSS Template

To install the template, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. Navigate to the project directory:
   ```
   cd your-repo-name
   ```
3. Install the dependencies:
   ```
   npm install
   ```

## Using Electron + Tailwind CSS Template

To use the template, follow these steps:

1. Build the CSS file:
   ```
   npm run build:css
   ```
2. Start the development server:
   ```
   npm run dev
   ```

This will start the Electron app with hot-reloading for both the main and renderer processes.

## Development Guidelines

- Main Process: Add any main process code to `main.js`
- Renderer Process: 
  - HTML: Edit `src/index.html` for your app's structure
  - CSS: Add custom styles to `src/assets/styles/styles.css`
  - JavaScript: Use `src/js/index.js` and `src/js/renderer.js` for renderer logic
- Assets: Place images and other static files in `src/assets/`

## Building for Production

To build the app for production and create an installer, we'll use Electron Forge. Electron Forge is already included in this template, so you don't need to install it separately. Follow these steps to create a distributable version of your app:

1. Make sure all your changes are saved and committed.

2. Run the following command to create a production build:
   ```
   npm run make
   ```

3. Electron Forge will create a `out` directory in your project folder. Inside, you'll find:
   - A packaged version of your app
   - An installer for your target platform (e.g., .exe for Windows, .dmg for macOS)

4. You can customize the build process by editing the `forge.config.js` file in the root of your project.

For more information on configuring Electron Forge, refer to the [Electron Forge documentation](https://www.electronforge.io/).
