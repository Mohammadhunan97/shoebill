# Thank you for using Shoebill.js:


### Features:
	* lightweight and modular authentication
	* already setup encryption and sessions
	* plugin and use different features such as local authentication, google authentication, facebook authentication, and more (coming soon)

### To install run the following command:
	* npm install shoebilljs -g

### To initially setup your project:
	* cd into_your_project
	* npm install
	* npm install express mongoose passport body-parser express-session ejs bcryptjs chalk 
	* shoebill start <entryfile.js> <~/the_absolute_path_of_your_local_repo> 
	* if all files (listed below) are not automatically generated, run the above command again


### Files that are created by shoebill start <entryfile.js> <~/the_absolute_path_of_your_local_repo>:
	* Note: by running shoebill start you will overwrite any existing files by the below names
	* model/user.model.js
	* config/displayroutes.js - this file is used simply for viewing the available routes in the terminal
	* routes/localuser.routes.js - this file is used for c.r.u.d functionalities for local users and to login
	* views/index.ejs - this file is a template file for your homepage, including instructions to include premade signup or login partials in this homepage
	* views/partials/signup.ejs - this file is a partial for a local signup form
	* views/partials/signup.ejs - this file is a partial for a local login form
	* views/profile.ejs - this file is a template file for your profile
	* public/shoebill.css - this file is the styling linked in views/index.ejs
	* ./<entryfile.js> - this file is created through the first parameter when you run shoebill start
	* /routes/user.routes.js - this file contains the routes shared amongst all users, regardless of whether they were created locally or through oauth/passport
	* ./key.js - this file contains the placeholder client_ids and secrets in the proper format, you must edit this file to use shoebill add <socialmedia>

### API:
	* shoebill start <entryfile> <absolute__local_project_path> | shoebill start app.js ~/tumblrclone
	* shoebill add <socialmedia> | shoebill add facebook, shoebill add google (not yet available)

### Goals:
* Make list all routes executable [ ]
* Make add facebook executable for oauth 2.0 sign in [ ]
* Make add google executable for oauth 2.0 sign in [ ]
* Add posts resource, including ejs layouts for posts, models for post, and routes for posts. [ ]
* Add email support  [ ]
* Make more similar to Devise [ ]