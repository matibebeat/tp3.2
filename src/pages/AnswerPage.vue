<script setup>

</script>

<template>
  <h1>Answer</h1>
  <h2>Here is the answer to the question</h2>
  <ol>
    <li>
      <h3>
        Webpack is internally used by the Vue CLI. WHY is it required to deal with both multiple js files and multiple .vue files?

      </h3>
      <p>
        Webpack is a module bundler that takes multiple files and bundles them into one file. It is required to deal with multiple js files because it allows you to use `import` and `export` statements to import and export modules. It is also required to deal with multiple `.vue` files because it allows you to use Vue single file components, which are `.vue` files that contain the template, script, and style for a component in a single file.
      </p>
    </li>
    <li>
      <h3> What is the role of Babel and how browserslist ay configure its outpu?
      </h3>
      <p>
        Babel is a JavaScript compiler that allows you to use the latest JavaScript features in your code and have it transpiled to older versions of JavaScript that are supported by most browsers. Browserslist is a configuration file that allows you to specify which browsers you want to target with your compiled code. Babel uses Browserslist to determine which browsers to target when transpiling your code.
      </p>

    </li>
    <li>
      <h3> What is ESLint and wich set of rules are currently applied?
      </h3>
      <p>
        ESLint is a static code analysis tool that helps you find and fix problems in your JavaScript code. It enforces a set of rules that help you write clean and consistent code. The rules that are currently applied can be found in the `.eslintrc.js` file in the root of the project.
      </p>
    </li>

    <li>
      <h3>what is the diffenrece between scoped style and non-scoped styles in Vue?</h3>
      <p>  Scoped styles are styles that are scoped to a specific component and do not affect other components. Non-scoped styles are global styles that affect all components in the application.</p>
    </li>

    <li>
      <h3>for the async button, why do we use finally and not then</h3>
      <p>  We use `finally` instead of `then` because `finally` is called after the promise is settled, whether it is resolved or rejected. This allows us to perform cleanup actions, such as hiding a loading spinner, regardless of the outcome of the promise.</p>
    </li>
  </ol>
</template>

<style scoped>

</style>