# CodeCraft

A React-based Code Pen clone that allows users to write HTML, CSS, and JavaScript in separate panels and see a live preview in real-time. Built as a front-end portfolio project to demonstrate editor integration, state management, and live preview rendering.

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen)](https://codepenproj.netlify.app)

---

## Table of Contents

- [Project Overview](#project-overview)
- [Live Demo](#live-demo)
- [Screenshots](#screenshots)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Project Structure](#project-structure)
- [Setup & Installation](#setup--installation)
- [Usage](#usage)
- [Future Improvements](#future-improvements)
- [Contact](#contact)

---

## Project Overview

**CodePen** replicates the core functionality of CodePen, providing three code editors (HTML, CSS, and JavaScript) with syntax highlighting and a live preview pane. This project demonstrates:

- Integration of CodeMirror in React.
- State management for editor content.
- Dynamic generation of an iframe `srcDoc` for live rendering.
- Responsive, collapsible editor panes.
- Use of React hooks, component composition, and CSS for layout.

It serves as a learning exercise and as a showcase piece for front-end/interview portfolios.

---

## Live Demo

Try the live version here:

👉 https://codepenproj.netlify.app

*(Hosted on Netlify; updates automatically upon merging to the main branch if configured.)*

---

## Screenshots


### Full Layout
![Full Layout Screenshot](./screenshots/FULLVIEW.png)

### Collapsed Editor Pane
![Collapsed Pane Screenshot](./screenshots/COLLAPSEDVIEW.png)

### Collapsed HTML Pane
![Collapsed Pane Screenshot](./screenshots/HTMLCOLLAPSED.png)

### Collapsed CSS Pane
![Collapsed Pane Screenshot](./screenshots/CSSCOLLAPSED.png)

### Collapsed JS Pane
![Collapsed Pane Screenshot](./screenshots/JSCOLLAPSED.png)

---

## Technologies Used

- **React** – Frontend library for building UI components.
- **CodeMirror** + **react-codemirror2** – Integrated code editor with syntax highlighting.
- **FontAwesome** – Icons for toggle buttons.
- **HTML5 / CSS3 / JavaScript (ES6+)** – Core web technologies.
- **Flexbox / CSS Grid** – Responsive layout for editor and preview panes.
- **Netlify** – Deployment of the static React app.

---

## Features

- **Three separate editors** for HTML, CSS, and JavaScript with syntax highlighting.
- **Live preview** pane that updates in real-time as you type (debounced for performance).
- **Collapsible editor panes**: focus on a particular language by expanding or collapsing panels.
- **Responsive design**: adapts to different screen sizes.
- **Sandboxed iframe** for rendering user code safely (`sandbox="allow-scripts"`).
- **Clean, minimal UI** resembling CodePen’s core experience.

---

## Project Structure


```text
├── myapp/                 # React project root
│   ├── node_modules/      # Installed dependencies
│   ├── public/            # CRA public files
│   ├── src/               # Source code folder
│   │   ├── components/    # Components folder
│   │   │   ├── App.js     # Main app component
│   │   │   └── Editor.js  # Code editor component
│   │   ├── hooks/         # Custom hooks folder
│   │   │   └── local.js   # Custom hook for localStorage
│   │   ├── index.css      # CSS styles for the project
│   │   └── index.js       # React app entry point
│   ├── .gitignore         # Files to exclude from git
│   ├── .nvmrc             # Node version (optional)
│   ├── package-lock.json  # Lock file for npm
│   ├── package.json       # Project metadata and scripts
├── README.md              # Project documentation
├── netlify.toml           # Netlify deployment configuration
├── screenshots/           # Folder to store project screenshots
```
---


## Setup & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/sakshiy16/CodeCraft.git
cd CodeCraft/myapp
```

### 2. Install Dependencies
```bash
Copy code
npm install
```
### 3. Run in Development Mode
```bash
npm start
```
The app will open automatically at http://localhost:3000.

### 4. Build for Production
```bash
npm run build
```
---


## Deploy to Netlify

- Connect your GitHub repository in Netlify.
- Set the build command to: `npm run build`
- Set the publish directory to: `myapp/build`
- Alternatively, drag and drop the `build/` folder into Netlify’s deploy panel.

👉 Live Demo: https://codepenproj.netlify.app
---


## Usage

- Open the app in your browser.
- Write **HTML** in the HTML editor.
- Write **CSS** in the CSS editor.
- Write **JavaScript** in the JS editor.
- The live preview pane will automatically update.

 ### The Combined Output:
 ```html
 <html>
  <body>...your HTML...</body>
  <style>...your CSS...</style>
  <script>...your JS...</script>
 </html>
```
- Use the collapse/expand buttons on each editor to focus on a specific pane.
---


## Future Improvements



- ✅ Auto-save code using localStorage.
- ✅ Support multiple pens with save/load functionality.
- ✅ Add user authentication to save and manage pens.
- ✅ Theme toggle: light and dark modes.
- ✅ Show JavaScript errors in a console panel.
- ✅ Allow adding external libraries like React, Bootstrap via CDN.
- ✅ Improve mobile responsiveness.
- ✅ Add accessibility support.
- ✅ Write unit and integration tests.

---


## Contact

**Author:** Sakshi Yadav  
**Email:** sakshiy1612@gmail.com  
**GitHub:** [sakshiy16](https://github.com/sakshiy16)

Feel free to connect for feedback, collaboration, or questions!

---

## License

This project is open source under the MIT License.
