<template>
  <nav class="navbar">
    <div class="navbar-menu">
      <div class="navbar-end">
        <router-link to="/home" class="navbar-item">Home</router-link>
        <router-link to="/about" class="navbar-item">About</router-link>
        <router-link to="/contact" class="navbar-item">Contact</router-link>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar'
};
</script>

<style scoped>

.navbar {
  background-color: #898989;
  padding: 1rem;
}

.navbar-brand {
  color: white;
  font-size: 1.5rem;
  font-weight: bold;
}

.navbar-item {
  color: white;
  margin-right: 1rem;
  cursor: pointer;
}

.navbar-item:hover {
  text-decoration: underline;
}
</style>
