<template>
  <main>
    <section>
      <ul></ul>
      <p class="no-tasks">No tasks yet!</p>
    </section>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { type Task } from '../Task'

export default defineComponent({
  name: 'main',
  data() {
    return {
      tasks: [] as Task[]
    }
  }
})
</script>

<style scoped>
section {
  padding: 0.5rem;
  max-width: 800px;
  margin: 0 auto;
}
.no-tasks {
  display: inline-block;
  text-align: center;
  font-size: 1.4rem;
  line-height: 3rem;
  margin-top: 2rem;
  width: 100%;
  height: 3rem;
  padding: 0.3rem 0.6rem;
  background-color: var(--primary-white);
  box-shadow: 8px 8px 24px -13px rgba(30, 30, 33, 0.39);
  border-radius: 10px;
}
</style>
