<template>
  <nav>
    <NavBar></NavBar>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/operation">Operation</router-link>
  </nav>
  <router-view />
  <Footer :myNumber="8"></Footer>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Footer from "@/components/Footer.vue";
import Operation from "@/components/Operation.vue";

export default {
  name: "App",
  components: {
    'NavBar': NavBar,
    'Footer': Footer,
    'Operation': Operation,
  }
}
</script>
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
