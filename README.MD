# Welcome To JSONMarkup from WebWorks

This is a simple bit of software that lets you create websites using JSON. It is not recommended for general use, but instead for code generation from software. So for example a website builder may use the syntax of JSONMarkup and then use this software to convert it to working HTML, CSS, and JS.

# Notice

The point of this repository is not to share the code, the code is free to use and republish or do what you want with (read licence), but it's not meant for people to edit and make there own versions.

# How to display the JSON as a website
## Clone the repository
Navigate to your coding space. Run the following command
`git clone https://github.com/MJDaws0n/JSONMarkup-PUBLIC.git`

## Create an index.html file
Create your main file, this will be the file that you will access to view the page. Set the contents of the file to the contents of the example preview code located at [/general/preview/displayWebsite.html](https://github.com/MJDaws0n/JSONMarkup-PUBLIC/blob/main/general/preview/displayWebsite.html).

## Modify the example code
On the first line set `../../main.js` in `src="../../main.js"` to the correct location of the main.js file. Then, set `../../main.js` in `import { compileWebsite } from '../../main.js';` to the correct main.js file location. The main js file will be at the base of the file directory set. Modify the `../../general/example/example.json` in `fetch('../../general/example/example.json')` to the correct location of your JSON script, it can be local or a file online.
