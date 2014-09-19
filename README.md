# Parsing and Displaying a Markdown File with CommonMark

## What's This Do?
Renders a markdown file as HTML and displays it. JavaScript loads a markdown file, parses it and displays it as HTML inside the index.html file. The index.html file includes 2 Javascript files:

* The first -- ```js/stmd.js``` -- loads the [CommonMark](http://commonmark.org) library which can convert CommonMark (standardized markdown) to HTML. 

* The second -- ```render.js``` -- loads a specified markdown file (default is ```README.md```) via XHR then parses it and renders it with the CommonMark JS library.

[See the demo](http://sawmac.github.io/display-markdown/)

## Why?
I wanted a way to display markdown files as HTML on any website -- but in particular, I wanted to be able to use Github pages to render the README.md file for a repo. Mainly so I could use a repo as a way to create installation guides and other how-to's in a single markdown file.

I also wanted a way that was backend agnostic so it could all be handled via JavaScript without any server requirements.

I know Github has a markdown API but I wanted to try out the CommonMark library

## How to use
1. Throw the ```index.html``` file into the same folder as the ```README.md``` (or other markdown file)
2. Add the ```js``` folder (or just place the ```render.js``` and ```stmd.js```) in the same folder as the index.html. You may need to adjust the paths if you move the js files or the markdown file is in a different directory than the index.html file.
3. Open the index.html file. (Uses XHR so you have to view through a web server).

## To do
1. Add more CSS to style this sucker better