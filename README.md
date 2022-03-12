# webPackProject

## Entry: 
    The entry point is simply a module or a JavatScript file (defaults to ./src/index.js) which webpack uses to start bundling. Webpack looks for the import statements in this module and builds the dependency graph of all the dependencies. If you don't use the default entry point i.e ./src/index.js, you need to specify it in the configuration file.

## Output: 
    Using the output point, you tell webpack the name and path of the file(s) where to produce the final bundle or set of bundles. By default it's ./dist/main.js for the main bundle and you can specify your custom values in the configuration file.

## Plugins: 
    Webpack can be extended with plugins which are used for adding features that cant' be imlemented using loaders.

## Flow our Webpack project:

- Initially here we created a folder for our project and initialized using **npm init -y**, this will create a package.json file in our project folder.
- Now we installed our webpack and webpack cli using **npm install webpack webpack-cli --save-dev**.
- To show the entry point for webpack we created src folder and index js file. Here to create js file we used **touch <js file name(index.js)>**
- Now we have to add a start under script which consists in package.json file **"start": "webpack --mode development"**.
- Now we run our webpack using **npm start**.
- After running our webpack there will be a dist folder with main.js file generated.
- Here we created our index html file and gave some basic code along with script tag mapping to our main.js file.
- Now to make everything dynamic we installed webpack plugin using **npm install html-webpack-plugin --save-dev**.
- Now we need to add the plugin to our webpack configuration file, so we created a webpack.config.js file in the root folder of your project using **touch webpack.      config.js**
- After creating the file, we declared our plugin inside the config js file.
- Now if we run our webpack there will be an index html file automatically generated in dist folder of our project.
- Now we have declare our entry point and output point for this project, whereas entry shows the starting point to execute and output shows the our bundle js file and path to be check.
- Now we can run our webpack in dynamic development mode.