# t-net

//Enviromental setup see ___

# Vue js project template
# https://github.com/vuejs/vue-cli
# create the client

   $ sudo npm install -g vue-cli
   $ vue init <template-name> <project-name>
   $ vue init webpack my-project

(vue-cli@2.9.1)

   > vue init webpack-simple client

   (server js was not build because used webpack-simple instead)

# install the dependecies inside our package.json file

   > npm update

   (install dependencies locally?)

# can now launch the html server

   > npm run dev

output: > client@1.0.0 dev /home/kevin/Desktop/t-net/client
> cross-env NODE_ENV=development webpack-dev-server --open --hot

Project is running at http://localhost:8080/
webpack output is served from /dist/
404s will fallback to /index.html

(w/e that means)

# commit changes to github

   > git add --all
   > git commit -m "added vue init cli with webpack-simple"

# create/add the server

    > mkdir server
    > cd server
    > sudo npm init -f      //create package.json
    > sudo npm install --save nodemon eslint        //install deprendencies, and update json file
   
# add dependencies, 

   > sudo npm install --save eslint
   # initailize eslint,  file is node_modules/eslint/bin/eslint.js
   > node ./node_modules/eslint/bin/eslint.js --init
   1. pick "use popular style guide" 2. "Standard" 3. "Javascript" 
  
   > sudo npm install --save nodemon


# add scripts in the package.json that make use of dependencies above

   1. "start": "./node_modules/nodemon/bin/nodemon.js src/app.js",  //creates command
   2. "lint": "./node_modules/.bin/eslint **/*.js"

# create the app.js inside of the server folder

   > mkdir src
   create app.js file with file exporeer in VS code

# run the app.js file we just make (currently only has console.log("hello") with a newline at the end)

    > npm start

(app.js is the main entry point)

# add express and other dependecies

   >sudo npm install --save express body-parser cors morgan

# around min 30 enviroment is kinda set up and can start bilding the app
# https://www.youtube.com/watch?v=Fa4cRMaTDUI


