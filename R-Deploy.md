# Deployment Notes  
 Development enviroment is set. These tasks are for deployment of site to a server.
# To Do
1. Have Sass output .min - IF Autoprefix accepts min file as source   
(All style editing is done in partials anyway.)

- Test if copy and paste of new project folder works out of box.
- Clean Up share-nodes folder 
- Custom gulp functions (In development no need for minify and compile)

# Order Deployment Steps
1. Files (Handled in Development cycle)     
    1. Compile HTML Includes (gulp-fileinclude)
    1. Move files to dist folder (gulp-fileinclude)
1. Javascript
    1. JavaScipt compile
    1. javaScript minify
    1. javascript error check
1. Stylesheets
    1. Autoprefix - Adds Browser fixes to css
    1. Minify - Output to .min file
1. Images
    1. Compress / Minify images
    1. SVG handling (If needed)

# Files
1. Compile: Gulp-fileinclude compiles html include files (partials) from /inc folder and outputs to /dist folder using *.html modifier to move Non-Compiled .html files to /dist folder.

# Javascript
- Compile
- Minify
- Error Check

# Styles / CSS
1. Dev: Sass & Live Sass extensions watch and auto compile partial files and ouputs to dist/css folder. 
- Autoprefix - Adds Browser fixes to css
- Minify - Output to .min file

# Images
- Compress / Minify images
- SVG handling (If needed)

# Installed
1. Git
1. Github
1. Sass
1. Gulp
    1. gulp-fileinclude

### Gulp Extensions to checkout
- [ ] gulp-sass
- [ ] gulp-cssnano
- [ ] autoprefixer
- [ ] autoprefixer by Aaron Russel https://aaron-russell.co.uk/blog/16-awesome-gulp-plugins/
- [ ] gulp-sourcemaps
- [ ] gulp-concat
- [ ] gulp-uncss
- [ ] gulp-uglify - Minify js files
- [x] gulp-fileinclude
- [ ] gulp-imagemin
- [ ] gulp-tinypng
- [ ] gulp-watch
- [ ] gulp-iconfont  
- [ ] gulp-eslint- Error check files (lint) 