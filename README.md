# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some Oxlint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the Oxlint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and Oxlint's TypeScript related rules in your project.


=================================================================
install vite to work on react  
    npm install -g create-vite
Creta project  using Vite 
    npm create vite@latest my-react-app
after that it will start running and you will get the url
    Local:   http://localhost:5173/


=====================deployment================================
create a repo directly from github and followed the steps mentioned over that

then

In the local in vite.config.js just add
    base: "/school/"

in the package.json add
    "homepage": "https://git-for-ankit.github.io/school",
    
    "scripts":{
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build" 
    }

and the run the below command in sequence
Adding the GitHub Pages dependency packages
    The gh-pages package allows us to publish the build file of our application into a gh-pages branch on GitHub, where we are going to host our application. Install the gh-pages dependency using npm :

    npm install gh-pages --save-dev

 Pushing the code updates to the GitHub repository and finally deploying the application

 Finally deploy the application using the following command in the terminal:    
    npm run deploy

This command will publish your application on the branch named gh-pages and can be opened by the link given in the homepage property written in the package.json file.

View the deployed app on GitHub
