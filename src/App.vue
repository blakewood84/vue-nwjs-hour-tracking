<template>
  <div id="app">
    <b-navbar toggleable="x-lg" type="dark" variant="info">

      <b-button v-b-toggle.sidebar>Menu</b-button>
      <b-navbar-brand href="#">NavBar</b-navbar-brand>
      
    </b-navbar>
    
    <b-sidebar id="sidebar" title="Menu" shadow>
      <div class="px-3 py-2">
        <b-list-group>
          <b-list-group-item b-link to='/'>
            Hours Log
          </b-list-group-item>
          <b-list-group-item b-link to='/projects'>
            Projects
          </b-list-group-item>
        </b-list-group>
        <div class='dropdown-divider'></div>
        <b-list-group>
          <b-list-group-item b-link to='/about'>
            Exports
          </b-list-group-item>
          <b-list-group-item b-link to='/about'>
            Settings
          </b-list-group-item>
        </b-list-group>
      </div>
    </b-sidebar>

    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
