# Pug-plugin issue (fixed in v4.9.7)

## Description

When you add a script from modules (like so: `script(src=require('bootstrap/dist/js/bootstrap.bundle.js'))`) 
and then when using webpack-dev-server you make changes in any .scss or .js file of the project you get this error in the browser's console:

`Not allowed to load local resource: file:///E:/pug-plugin-issue/node_modules/bootstrap/dist/js/bootstrap.bundle.js`

## How to reproduce

1. Clone, install and start
```
git clone https://github.com/jeneko/pug-plugin-issue

cd pug-plugin-issue

npm i

npm start
```
2. Open <a href="http://localhost:8080" target="_blank">localhost:8080</a> in your browser
2. Open browser's console
2. Make any change in any .scss file of the project
2. Get error in console

![error-image](https://user-images.githubusercontent.com/16610240/222920964-bf9c21de-702d-4734-bb97-22122c96eaa6.png)
