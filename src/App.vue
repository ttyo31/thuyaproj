<template>
  <nav style="padding: 0%;">
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
    <div style="background-color: #eae2d6;">
    <nav class="navbar navbar-expand-lg navbar-light custom-navbar">
      <router-link class="navbar-brand" to="/" style="color: #063970;">MyPortfolio</router-link>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <router-link class="nav-link" to="/" exact>Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/work">Past Jobs</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/experience">Enriching Experiences</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/hobbies">Hobbies</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/contact">Contact</router-link>
          </li>
        </ul>
      </div>
    </nav>
  </div>
  </nav>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
