## Frontend ~/.dotfiles

To keep consistency to the style of frontend resources, I decided to stick to some shared rules that have to be applied to every project using some editors plugins.

#### Basic Editor Configuration
I chose to use [EditorConfig](http://editorconfig.org/) to share the basic configuration like indentation and charset. It works including an `.editorconfig` file in the root directory and making sure your editor has the necessary plugin. You can find a list of downloads [here](http://editorconfig.org/#download). The choice to keep the indentation with 2 spaces is to be compliant with actual standards (major frameworks use this configuration both for JS and CSS).

#### Auto correction on save
I have chose to use [js-beautify](https://github.com/beautify-web/js-beautify). Despite of his name it works as a beautifier also for HTML and CSS. Every editor has a plugin that implement it, es. [Sublime](https://github.com/victorporof/Sublime-HTMLPrettify) or [Atom](https://atom.io/packages/atom-beautify). The setup for js-beautify is controlled within a `.jsbeautifyrc` file that have to be included in the root directory of the project. For now I decided to auto correct SCSS and JS files, .hbs are not completely supported yet.

#### JS Hint
To check on JavaScript syntax we use [JSHint](http://jshint.com/). The rules to detect errors are written in a `.jshintrc` file included in the root directory of the project.

#### Eslint
To check on Javascript / React [.js / .jsx] syntax we use [Eslint](http://eslint.org/). The rules to detect errors are written in a `.eslintrc` file included in the root directory of the project.
