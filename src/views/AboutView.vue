<template>
  <div class="about">
    <h2>This is an about page, which takes props from parent</h2>
    <Children :message="parentMessage" />
    <p>{{ parentMessage }}</p>
  </div>
  <input v-model="parentMessage" />
</template>

<script>
import Children from '@/components/aboutUs/Children.vue'

export default {
  components: {
    Children,
  },

  data() {
    return {
      parentMessage: 'This is info from parent passed to prop',
    }
  },

  methods: {
    dataPassed() {
      console.log(`This is passed message to children component ${this.pare}`)
    },
  },
}
</script>
