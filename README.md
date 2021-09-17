# new-project-template
A project to create a new project template.
## Added Git
Created repo on Github.  
Used clone ssh_url to clone to local folder.  
It added hidden .git folder.  
EXPECTED: It did not create a remote file "adds remote"  
## Added Sass
Checked if Sass enabled using: sass --version .  
Result: Term Sass not recognized.  
Created package.json using the command: npm init .  
Result: File looks like it should have been created in Git setup.  
Ran command: npm install -g sass .  
Result: Sass installed.  
## Added Sass Dependancy
Ran command: npm install node-sass .  
Result: Added dependancy to .json file and added node-modules folder with references to existing in it.  
TODO: After working try to delete node modules folder. (Copy folder to master nodes folder so we have full version with all extensions added.)  
## Test Sass
In .json files changed test to: "scripts": {"sass": "node-sass -w scss/ -o css/ --recursive"} .  
Ran test using command: npm run sass .  
Result: Error - scss folder not found  
Created scss folder  
Ran test using command: npm run sass .  
Result: No error. Assume it's working.  
## Real Sass Test
Added _color.scss.  
Added test.scss.  
Ran Watch Sass  
Sass created folder and included node modules.  
Added ignore node module folder to sass live extensions global exclude "**/node_modules/**".  
Result: PASSED  
Deleted nodes module folder (Maybe too early since I did not add gulp and extensions yet).  
## Install Gulp
Check for node: node --version (passed)  
Check for npm: npm --version (passed)  
Check for npx: npx --version (passed)  
Instal command line utility: npm install --global gulp-cli (skipped)  
Navigated to project folder.  
Create package.json: npm: init (skipped)  
Install package dependancies: npm install --save-dev gulp  
Result: Gulp dependancy added to package.json. Created .gitignore from prompt to ignore re-installed node_modules.  
Check Gulp version: gulp --version  
Result: Version is now CLI version. (passed)  
## Test Gulp
Create file gulpfile.js  
Run command: gulp  
Result: PASSED
## Gulp Extentions
