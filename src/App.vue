<template>
  <div>
    <div id="nav">
      <router-link :class="{ active: $route.name === 'Home' }" to="/"
        >Home</router-link
      >
      |
      <router-link :class="{ active: $route.name === 'Cart' }" to="/cart"
        >Cart</router-link
      >
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

html,
body {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
body {
  background-color: white;
}

#nav {
  padding: 10px;
  width: 100%;
  height: 35px;
  background-color:blanchedalmond;
  line-height: 30px;

  a {
    font-weight: bold;
    color: darkgray;
    text-decoration: none;
    margin: 0 5px;
    font-size: 1.25rem;

    &.active {
      color: green;
    }
  }
}

.text-center {
  text-align: center;
}
</style>
