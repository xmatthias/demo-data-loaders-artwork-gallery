<script setup lang="ts">
const somethingStr = something()
</script>

<template>
  <header>
    <div class="wrapper">
      {{ something() }}
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
