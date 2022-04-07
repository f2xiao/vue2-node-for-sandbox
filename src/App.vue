<template>
  <div id="app">
    <h1 class="text-3xl font-bold underline">Hello world!</h1>
    <ul class="list-disc list-inside">
      <li>One</li>
      <li>Two</li>
      <li>Three</li>
    </ul>
    <ul role="list">
      <li>One</li>
      <li>Two</li>
      <li>Three</li>
    </ul>
    <img src="@/assets/logo.png" alt="logo" />
  </div>
</template>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
