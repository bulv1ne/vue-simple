<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>\{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  data{{#if_eq lintConfig "standard"}} {{/if_eq}}() {
    return {
      msg: 'Hello Vue!'{{#if_eq lintConfig "airbnb"}},{{/if_eq}}
    }{{#if_eq lintConfig "airbnb"}};{{/if_eq}}
  }{{#if_eq lintConfig "airbnb"}},{{/if_eq}}
}{{#if_eq lintConfig "airbnb"}};{{/if_eq}}
</script>

<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>
