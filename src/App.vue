<template>
  <div id="app">
    <nav id="nav" class="navbar navbar-light bg-light">
    <a class="navbar-brand" href="#">
      <img src="@/assets/myfinances.png" 
      alt="" 
      width="30" 
      height="24" 
      class="d-inline-block align-text-top">
      MyFinances
    </a>
      <router-link to="/">Home</router-link> |
      <router-link to="/signup">Registracija</router-link> |
      <router-link to="/login">Prijava</router-link>
    </nav>
    <div class="container-fluid">
    <router-view />
    </div>
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

#nav {
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
