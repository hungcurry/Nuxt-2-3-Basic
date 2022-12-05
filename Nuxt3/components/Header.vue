<script setup>
</script>
<template>
  <div>
    <nav>
      <NuxtLink to="/">index</NuxtLink>
      <NuxtLink to="/:id">id</NuxtLink>
      <NuxtLink to="/window">window</NuxtLink>
      <NuxtLink to="/async">async</NuxtLink>
      <NuxtLink to="/fetch">Fetch</NuxtLink>
      <NuxtLink to="/router">router</NuxtLink>
    </nav>
  </div>
</template>
<style lang='scss' scoped>
a {
  display: inline-block;
  padding: 20px 10px;
  text-decoration: none;
  font-size: 24px;
  color: aqua;
}
</style>

