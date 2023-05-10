<script setup lang="ts"></script>

<template>
  <header class="header">
    <div class="container">
      <h1>{{ title }}</h1>
      <p>{{ description }}</p>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      title: 'To do App',
      description: 'Never forget again'
    }
  }
}
</script>

<style scoped>
.header {
  text-align: center;
  width: 100%;
  padding: 2rem;
  background-color: rgb(92, 127, 223);
}
.header h1 {
  color: var(--primary-white);
  font-size: 2.4rem;
  margin-bottom: 1rem;
}
.header p {
  color: var(--primary-black);
  font-size: 1.2rem;
}
</style>
