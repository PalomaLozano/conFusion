<h2>conFusion</h2>


<b>In this project we used the following tools:</b>

Node.js
-> To install Node on your machine, go to https://nodejs.org and click on the Download button. Depending on your computer's platform (Windows, MacOS or Linux), the appropriate installation package is downloaded.

-> Initializing package.json: npm init

-> Follow along the prompts and answer the questions as follows: accept the default values for most of the entries, except set the entry point to index.html

-> This should create a package.json file

-> Install an NPM module, lite-server, that allows you to run a Node.js based development web server and serve up your project files. To do this, type the following at the prompt: npm install lite-server --save-dev

->Next, open package.json in your editor and modify it as shown below:

"scripts": { "start": "npm run lite", "test": "echo "Error: no test specified" && exit 1", "lite": "lite-server" },

-> start the development server by typing the following at the prompt: npm start

-> This should open your index.html page in your default browser.

Setting up .gitignore
-> Next, create a file in your project directory named .gitignore (Note: the name starts with a period)Then, add the following to the .gitignore file: node_modules

-> Then do a git commit and push the changes to the online repository. You will note that the node_modules folder will not be added to the commit, and will not be uploaded to the repository.

Bootstrap
-> Go to a convenient folder location on your computer and download the Bootstrap4-starter.zip file using the link provided at the top of this page.

-> Unzip the file to see a folder named Bootstrap4 and a sub-folder under it named conFusion created. Move to the conFusion folder.

-> Open a cmd window/terminal and move to the conFusion folder.

-> At the prompt type: npm install

-> This will install the lite-server node module to your project.

-> Next, initialize a Git repository in the project folder, and then set up a .gitignore file with the contents as shown below: node_modules

-> You will use npm to fetch the Bootstrap files for use within your project. Thereafter you need to install JQuery and Popper.js as shown below since Bootstrap 4 depends on these two. At the prompt, type the following to fetch Bootstrap files to your project folder:

npm install bootstrap@4.0.0 --save

npm install jquery@3.3.1 popper.js@1.12.9 --save

-> Insert the following code in the of index.html file before the title.

<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
<meta http-equiv="x-ua-compatible" content="ie=edge">


<!-- Bootstrap CSS -->
<link rel="stylesheet" href="node_modules/bootstrap/dist/css/bootstrap.min.css">
-> At the bottom of the page, just before the end of the body tag, add the following code to include the JQuery library, popper.js library and Bootstrap's Javascript plugins. Bootstrap by default uses the JQuery Javascript library for its Javascript plugins. Hence the need to include JQuery library in the web page.

<script src="node_modules/jquery/dist/jquery.slim.min.js"></script>
<script src="node_modules/popper.js/dist/umd/popper.min.js"></script>
<script src="node_modules/bootstrap/dist/js/bootstrap.min.js"></script>
