<template>
  <section>
    <nav
      id="nav"
      class="navbar"
      role="navigation"
      aria-label="main navigation"
      style="width: 100vw"
    >
      <div class="navbar-brand">
        <a class="navbar-item" href="/">
          <img src="~/assets/ic_logo.png" alt="Velox" />
        </a>

        <a
          role="button"
          class="navbar-burger burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="navbarBasicExample"
          v-on:click="showNav = !showNav"
          v-bind:class="{ 'is-active': showNav }"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div
        id="navbarBasicExample"
        class="navbar-menu"
        v-bind:class="{ 'is-active': showNav }"
      >
        <div class="navbar-end">
          <div class="navbar-item">
            <a class="navbar-item is-transparent" v-scroll-to="'#screenshots'">
              About Us
            </a>

            <a class="navbar-item is-orange">Get Started</a>
          </div>
        </div>
      </div>
    </nav>
  </section>
</template>

<script>
export default {
  data() {
    return {
      showNav: false,
    };
  },
};
</script>

<style scoped>
.navbar {
  background-color: #3b1a45;
  padding: 5px 100px;
}

.is-transparent {
  background-color: transparent;
  color: white;
  border: none;
}

.is-orange {
  background-color: #ff5724;
  border-radius: 4px;
  color: white;
  margin-left: 10px;
}
</style>