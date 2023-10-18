<template>
  <div class="Home">
    <router-link to="/">
      <img alt="Vue logo" src="./assets/Logo.jpg" height="100">
    </router-link>

  </div>
  <nav>
    <router-link to="/" class="nav-link">ARTWORK</router-link>
    <router-link to="/about" class="nav-link">ABOUT</router-link>
  </nav>
  <router-view />


</template>

<style lang="scss">
#app {
  font-family:worksans;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

}
.Home {
  text-align: center;
}

nav {

  text-align: center;
  margin-top: 15px;
}

.nav-link {
 
  font-size: 20px;
  color: #717070;
  margin: 20px;
  justify-content: center;
  text-decoration: none; /* Remove the default underline */
  transition: color 0.3s ease; /* Add a smooth color transition on hover */
}

.nav-link:hover {
  color: rgb(0, 0, 0); /* Change the color on hover */
}

/* Add an underline to the active link */
.nav-link.router-link-exact-active {
  text-decoration: underline;
  text-underline-offset: 7px;
  text-decoration-thickness: 1px;

}

</style>



