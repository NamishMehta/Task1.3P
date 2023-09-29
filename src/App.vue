<script setup>
import { RouterLink, RouterView } from "vue-router";
import FooterComponent from "./components/FooterComponent.vue";
</script>

<template>
  <div class="nav-container">
    <input type="checkbox" id="menu-toggle" class="menu-toggle" />
    <label for="menu-toggle" class="dropdown-btn">Menu</label>
    <div class="links-container">
      <RouterLink class="nav-link" to="/">Home</RouterLink>
      <RouterLink class="nav-link" to="/about">About</RouterLink>
      <RouterLink class="nav-link" to="/resume">Resume</RouterLink>
      <RouterLink class="nav-link" to="/contact">Contact Us</RouterLink>
    </div>
  </div>

  <div class="page-container">
    <div class="content-wrapper">

      <RouterView />
    </div>
    <footer class="amazing-footer">
      
      <FooterComponent />
    </footer>
  </div>
</template>

<!-- 
<template>
  <div class="nav-container">
    <input type="checkbox" id="menu-toggle" class="menu-toggle">
    <label for="menu-toggle" class="dropdown-btn">Menu</label>
    <div class="links-container">
      <RouterLink class="nav-link" to="/">Home</RouterLink>
      <RouterLink class="nav-link" to="/about">About</RouterLink>
      <RouterLink class="nav-link" to="/contact">Contact Us</RouterLink>
    </div>
  </div>

  <RouterView />

  <FooterComponent/>
</template> -->

<style scoped>
/* Add this to your styles */
.page-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh; /* This ensures the container takes at least the full height of the viewport */
}

.content-wrapper {
  flex: 1; /* This makes the content take up all available space, pushing the footer to the bottom */
}

.nav-container {
  display: flex;
  justify-content: center;
  background-color: grey;
  padding: 10px 0;
  position: relative;
  flex-wrap: wrap;
}

.nav-link {
  text-decoration: none;
  color: #ecf0f1;
  padding: 10px 20px;
  margin: 0 10px;
  font-size: 1.1em;
  transition: background-color 0.3s, color 0.3s;
  border-radius: 4px;
}

.nav-link:hover {
  background-color: black;
  color: #bdc3c7;
}

.router-link-active {
  color: white;
  background-color: black;
  border-radius: 4px;
}

/* Mobile styles */
.menu-toggle {
  display: none; /* hide the checkbox */
}

.dropdown-btn {
  display: none;
  background-color: grey;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  border-radius: 4px;
}

.links-container {
  display: flex;
}

/* Media query for small screens */
@media (max-width: 768px) {
  .dropdown-btn {
    display: block;
  }

  .links-container {
    display: none;
    flex-direction: column;
    position: absolute;
    top: 100%;
    left: 0;
    right: 0;
    background-color: grey;
  }

  .menu-toggle:checked + .dropdown-btn + .links-container {
    display: flex;
  }
}
</style>
