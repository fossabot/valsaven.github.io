<template>
  <div id="app">
    <header>
      <h1><a href="/" class="transparent-link" title="Val Saven. Full-Stack Developer">Val Saven</a></h1>
      <h2>Full-Stack Developer</h2>
    </header>
    <router-view></router-view>
  </div>
</template>

<script>
  export default {
    name: 'app',
  };
</script>

<style>
  #app {
    font-family: 'Source Code Pro', monospace;
    text-align: center;
    margin-top: 60px;
  }

  a,
  body {
    color: rgba(255, 255, 255, .5);
  }

  * {
    margin: 0;
    padding: 0;
  }

  html {
    font-size: 15px;
  }

  body,
  html {
    height: 90%;
    min-height: 90%;
  }

  body {
    display: flex;

    padding: 2em 2em 4em;

    cursor: default;
    text-transform: lowercase;

    background: #222;

    font-family: 'Source Code Pro', monospace;
    font-weight: 400;
    line-height: 1.3;

    align-items: center;
    justify-content: center;
  }

  @media screen and (max-width: 767px) {
    body {
      padding: 1.5em 1.5em 2em;

      font-size: 1.1em;
    }
  }

  a {
    transition: .3s;
    text-decoration: none;
  }

  a:hover {
    color: #fff;
    cursor: pointer;
  }

  a:focus {
    outline: 0;
  }

  .transparent-link {
    cursor: inherit;
    transition: none;

    color: inherit;
  }

  .transparent-link:hover {
    color: inherit;
  }

  h1,
  h2,
  h3 {
    font-size: 1em;
    font-weight: inherit;
    color: #fff;
  }

  header h1 {
    margin-bottom: .1em;

    font-family: Roboto, sans-serif;
    font-size: 2em;
    font-weight: 700;
    line-height: 1;
  }

  header h1 {
    display: inline-block;
  }
</style>
