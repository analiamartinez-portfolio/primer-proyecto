<template>
  <div id="app">
    <div id="nav">
      <b-container>
        <b-row class="nav-size" align-h="between" align-v="end">
          <b-col sm="1">
            <img width="90%" src="./assets/udemyRojoLogo.webp" alt="udemyRojo" />
          </b-col>
          <b-col sm="2">
            <router-link to="/">Home</router-link>
            <router-link to="/services">Services</router-link>
            <router-link to="/about">About</router-link>
          </b-col>
        </b-row>
      </b-container>
      <br />
    </div>
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
  padding: 40px;
}

#nav a {
  font-weight: bold;
  color: black;
  margin-right: 10px;
  margin-left: 16px;
  text-decoration: none;
}

#nav a.router-link-exact-active {
  color: #5624d0;
}

.nav-size {
  font-size: 18px;
}
</style>
