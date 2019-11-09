<template>
  <nav class="navbar navbar-expand-md navbar-light fixed-top py-4" id="main-nav">
    <div class="container">
      <a href="home" class="navbar-brand">
        <img src="../../src/assets/img/mlogo.png" width="50" height="50" alt="logo">
        <h3 class="d-inline align-middle">Mizuxe</h3>
      </a>
      <button class="navbar-toggler" data-toggle="collapse" data-target="#navbarCollapse">
        <span class="navbar-toggler-icon"></span>
      </button>
                <div class="collapse navbar-collapse" id="navbarCollapse">
            <ul class="navbar-nav ml-auto">
              <li class="nav-item" v-for="(value, name, index) in items" :key="index">
                <span
                  @click="selectItem(value)"
                  class="nav-link"
                  style="cursor: pointer;"
                >{{ name }}</span>
              </li>
            </ul>
          </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      items: {
        Home: "#home",
        About: "#about",
        "Meet the Author": "#authors",
        Contact: "#contact"
      }
    }
  },
  methods: {
    selectItem(item) {
      if (item === "#home")
        scrollTo({top: 0, behavior: "smooth"})
      else 
        document.querySelector(item).scrollIntoView({ behavior: "smooth", block: "center"})
    }
  }
};
</script>

<style>
</style>