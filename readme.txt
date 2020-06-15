Getting Started with REACT

Install Create React App to be easily build react apps
npm -g create-react-app

Add simple react snippets extension in vscode
add prettier extension in vscode

file > preferences > format on save should be true.

create-react-app creates an app with development server, webpack and babel.
these dependencies are hidden in react-app dependencies so you don\t have to deal with them.
if you want to edit the dependencies use npm eject


npm start will start the app

created in the public folder is index.html with links to manifest.json that describes attributes of application
this creates a div with id="root" in index.html
this is the container for the react application


created in the src folder.
app.js describes a component that then gets drawn in the page

In this hello World app, all the files created by create-react-app in src folder are deleted and
the index.js file is created.

const element = <h1>Hello World</h1> is a jsx expression that gets converted by webpack to
React.createElement element....
check it out at babel.js
the element is part of the virtual Dom
ReactDOM.render(element, document.getElementById("root")) renders it in the real DOM


-------------------------------------------------------------------------------

Custom Configs

In package.json you see the following as dependencies:
"dependencies": {
    "@testing-library/jest-dom": "^4.2.4",
    "@testing-library/react": "^9.3.2",
    "@testing-library/user-event": "^7.1.2",
    "react": "^16.13.1",
    "react-dom": "^16.13.1",
    "react-scripts": "3.4.1"
  },
  
the last three of these actually encompass all of webpack and babel.
to see the tools inside use npm eject
You can create custom configs by doing this but we are not going there


