# Installation Instruction

## Initial Setup

First, pull down the repo to a local repository.

Make sure you have the latest version of Node.js downloaded (the lastest version includes NPM).
__https://nodejs.org/en/download/__

Open terminal and change directory to the location of the framework (eg __CD ./squiz/clients/example/framework__). 
Make sure you're in the directory that contains package.json.

In terminal, run the command
```
npm init
```

Follow the installation setup prompts, you can change the following:
- package name
- description
- keywords
- author


Make sure you leave the rest as default so that all the package files are installed properly.


After the initial setup of the framework type the following into terminal
```
npm install
```
This command will do the following:

- Generate and build the initial distribution files - __/dist/js/main.js__, __/dist/css/styles.css__, __/dist/html/index.html__
- Start watching the __/src/*__ directory for any file changes and re-compile them
- Open your default browser and initiate live reload

If you want to run additional commands such as compiling just the Javascript or Stylesheets, you can open the package.json file and inspect
the commands that can be run in the terminal.

Some useful commands would be 
```
npm run watch:all
npm run build:all
npm run build:css
npm run build:js
npm run build:html
```
Once you've setup the framework for your new build, *commit* and *push* the project to a __new__ git repository you have setup for this project.

__Do not push your changes to the main framework repository!__

Using the following command in terminal will add eslint to the project, and saves it into the package.json file as a dev dependency
```
npm install --save-dev eslint
```
Additionally you can use a shorter command such as
```
npm i -D eslint
```

For more information on how to install new plugins or create new commands to run within your project visit the following link
https://css-tricks.com/why-npm-scripts/



