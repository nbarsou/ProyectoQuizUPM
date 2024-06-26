# Skeleton

These commands are used to quickly set up and start a new Express.js web application:

1. `npm init -y`: Initializes a new Node.js project with default values.
2. `npm install express-generator`: Installs the Express application generator globally.
3. `npx express --help`: Displays help information about the express command.
4. `npx express --view ejs miniproject`: Generates a new Express.js application named "miniproject" with the EJS view engine.
5. `cd miniproject`: Changes the current directory to the newly created Express.js application directory.
6. `npm install`: Installs dependencies for the Express.js application.
7. `npm start`: Starts the Express.js application.

# Supervisor

1. `npm install --save supervisor`: Installs the supervisor for the project, the `--save` option adds it to the dependencies file but had to add manually for it to work.

# Modify the home page

- To change the javascrip, change "routes/[name].js"
- To cahnge the html, change "views/[name].js"

# Add a favicon

- Make a favicon, added to public directory
- Install `npm install serve-favicon`
- Add to `app.js` with the follwing lines:
  - `var favicon = require('serve-favicon');`
  - `app.use(favicon(path.join(__dirname, 'public', 'favicon.ico')));`

# Add application layout

- Install `npm install express-partials`
- Add to `app.js` with the following lines:
  - `var partials = require('express-partials');`
  - `app.use(partials());`
- Leave only the body in the .ejs, like index.ejs
- Create `views/layout.ejs` with the layout for the rest of the html code.
