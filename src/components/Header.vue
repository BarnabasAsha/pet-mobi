<template>
  <header>
    <div class="header">
      <div class="header_logo">
        <img src="../assets/images/logo.png" alt="Pet Mobi" />
      </div>
      <nav class="header_nav">
        <ul>
          <li><a href="#">How it works</a></li>
          <li><a href="">Our Services</a></li>
          <li><a href="">About Us</a></li>
        </ul>
        <div class="header_btn">
          <a href="">Download App</a>
        </div>
      </nav>
      <button
        @click="() => (status = !status)"
        class="header_menu"
        :class="status ? 'active' : ''"
      >
        <span></span>
        <span></span>
        <span></span>
      </button>
    </div>
  </header>
  <MobileNav v-if="status" />
</template>

<script>
import MobileNav from "./MobileNav.vue";
import { ref } from "vue";

export default {
  name: "Header",
  components: {
    MobileNav,
  },
  setup() {
    const status = ref(false);
    return { status };
  },
};
</script>

<style lang="scss" src="../styles/header.scss"></style>
