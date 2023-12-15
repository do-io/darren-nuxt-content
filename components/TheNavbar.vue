<script setup>
const isMobileNavOpen = ref(false)
</script>

<template>
  <nav class="navbar">
    <div class="container">
      <div class="navbar-brand">
        <nuxt-link to="/" class="navbar-item has-text-weight-bold is-size-5">
          <Logo />
        </nuxt-link>
        <nuxt-link to="/about" class="navbar-item has-text-weight-bold is-size-5">
          About DO
        </nuxt-link>
      </div>
    </div>
  </nav>
</template>

<style>
.navbar-item img {
  max-height: inherit;
}
</style>
