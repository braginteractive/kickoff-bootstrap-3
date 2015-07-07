Kickoff - Bootstrap 3
===

Kickoff is a fork of Automattic's [_s](https://github.com/Automattic/_s) WordPress starter theme that includes Gulp and Bower. 

# Pre-Installation

Basic knowledge of the command line and the following dependencies are required to use kickoff:

- Node ([http://nodejs.org/](http://nodejs.org/)) -`npm install`
- Gulp ([http://gulpjs.com/](http://gulpjs.com/)) - `npm install --global gulp`
- Bower ([http://bower.io/](http://bower.io/)) -`npm install -g bower`


## Manual Installation

##### 1) Navigate to the /themes folder of your project
`cd /your-project/wordpress/wp-content/themes`

##### 2) Clone

`git clone https://github.com/braginteractive/kickoff-bootstrap-3.git`

##### 3) Find & Replace

You'll need to change all instances of the names: `kickoff` to your project name.

- Search for: `'kickoff'` and replace with: `'project-name'` (inside single quotations) to capture the text domain
- Search for: `kickoff_` and replace with: `project-name_` to capture all the function names
- Search for: `Text Domain: kickoff` and replace with: `Text Domain: project-name` in style.css
- Search for (and include the leading space): <code>&nbsp;kickoff</code> and replace with: <code>&nbsp;Project Name</code>(with a space before it) to capture DocBlocks
- Search for: `kickoff-` and replace with: `project-name-` to capture prefixed handles

##### 4) Install Gulp and Dependencies
- Run `npm install && bower install` from the command line to install Gulp and pull down any dependencies via Bower.

That's it! Now you can begin using Gulp.

# Usage
After you've installed kickoff, and run `npm install` and `gulp` from the command line you can start using gulp.

## Gulp

##### 1) Navigate to your new theme
`cd /your-project/wordpress/wp-content/themes/your-new-theme`

##### 2) Gulp tasks available:

`gulp` - Installs Bower Components and Font Awesome

`gulp watch` - Automatically handle changes to CSS, javascript, php, and image optimization. Also Livereload!

`gulp scripts` - Concatenate and minify javascript files

`gulp sass` - Compile, prefix, and minify CSS files

`gulp bower` - Install bower components

`gulp icons` - creates /fonts/ directory and adds Font Awesome font files