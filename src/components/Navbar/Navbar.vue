<template>
  <ul class="navbar" v-if="isOpen">
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
  </ul>
  <p v-else="">Nothing to display here</p>
  <button @click="setIsOpen">Open/Close Menu</button>
</template>

<script>
export default {
  data() {
    return {
      isOpen: true,
    }
  },

  methods: {
    setIsOpen() {
      this.isOpen = !this.isOpen
    },
  },
}
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  list-style: none;
  padding: 0;
  margin: 0;
  gap: 2rem;
  width: 100%;
}
</style>
