# Welcome To JSONMarkup from WebWorks

This is a simple bit of software that lets you create websites using JSON. It is not recommended for general use, but instead for code generation from software. So for example a website builder may use the syntax of JSONMarkup and then use this software to convert it to working HTML, CSS, and JS.

# Notice

The point of this repository is not to share the code, the code is free to use and republish or do what you want with (read licence), but it's not meant for people to edit and make their own versions.

# Docs
## How to display the JSON as a website
### Clone the repository
Navigate to your coding space. Run the following command
`git clone https://github.com/MJDaws0n/JSONMarkup-PUBLIC.git`

### Create an index.html file
Create your main file, this will be the file that you will access to view the page. Set the contents of the file to the contents of the example preview code located at [/general/preview/displayWebsite.html](https://github.com/MJDaws0n/JSONMarkup-PUBLIC/blob/main/general/preview/displayWebsite.html).

### Modify the example code
On the first line set `../../main.js` in `src="../../main.js"` to the correct location of the main.js file. Then, set `../../main.js` in `import { compileWebsite } from '../../main.js';` to the correct main.js file location. The main js file will be at the base of the file directory set. Modify the `../../general/example/example.json` in `fetch('../../general/example/example.json')` to the correct location of your JSON script, it can be local or a file online.

### Access the file
To visit your site, put it on a local server or another type, and access the HTML file you created. Your site will then load, you can then make changes to your JSON file and the site will update after a refresh. JSONMarkup tends to take a second to load so you might find better speed by exporting the site to HTML before publishing, this gives speed, at the cost of ease of access. See how to do that [here](#how-to-return-the-html-from-the-json-to-use-elsewhere)

## How to return the HTML from the JSON to use elsewhere
### Clone the repository
Navigate to your coding space. Run the following command
`git clone https://github.com/MJDaws0n/JSONMarkup-PUBLIC.git`

### Create an index.html file
Create your main file, this will be the file that you will access to view the page. Set the contents of the file to the contents of the example preview code located at [/general/preview/displayHTML.html](https://github.com/MJDaws0n/JSONMarkup-PUBLIC/blob/main/general/preview/displayHTML.html).

### Modify the example code
On the first line set `../../main.js` in `src="../../main.js"` to the correct location of the main.js file. Then, set `../../main.js` in `import { compileWebsite } from '../../main.js';` to the correct main.js file location. The main js file will be at the base of the file directory set. Modify the `../../general/example/example.json` in `fetch('../../general/example/example.json')` to the correct location of your JSON script, it can be local or a file online.

### Choose how to handle the HTML
There is a function that is run called `compileWebsite`. In the `compileWebsite` function, there is a callback that is set up as a default in the file, the example code runs `document.getElementById('code').textContent = HTML;` which shows the HTML on the screen, you may modify the code in there for your needs, the variable `HTML` is the variable that contains the HTML for the generated site, the HTML at the bottom of the example file is not required and is only there for the example.

# How to write JSON markup 
