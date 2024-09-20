## Webpack is internally used by the Vue CLI. WHY is it required to deal with both multiple js files and multiple .vue files?

Webpack is a module bundler that takes multiple files and bundles them into one file. It is required to deal with multiple js files because it allows you to use `import` and `export` statements to import and export modules. It is also required to deal with multiple `.vue` files because it allows you to use Vue single file components, which are `.vue` files that contain the template, script, and style for a component in a single file.


## What is the role of Babel and how browserslist ay configure its outpu?

Babel is a JavaScript compiler that allows you to use the latest JavaScript features in your code and have it transpiled to older versions of JavaScript that are supported by most browsers. Browserslist is a configuration file that allows you to specify which browsers you want to target with your compiled code. Babel uses Browserslist to determine which browsers to target when transpiling your code.

## What is ESLint and wich set of rules are currently applied?

ESLint is a static code analysis tool that helps you find and fix problems in your JavaScript code. It enforces a set of rules that help you write clean and consistent code. The rules that are currently applied can be found in the `.eslintrc.js` file in the root of the project.


# Exercise 2:

