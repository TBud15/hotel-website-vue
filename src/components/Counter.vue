<template>
  <div class="counter-div">
    <h1>{{ count }}</h1>
    <div class="buttons-div">
      <button @click="increment" class="increment-button">Increment Counter</button>
      <button @click="decrement" class="decrement-button">Decrement Counter</button>
      <button @click="reset" class="reset-button">Reset Counter</button>
    </div>
    <form class="input-div" @submit.prevent="submitForm">
      <p>Set counter to:</p>
      <input type="text" id="num" v-model="submittedCount" />
      <button type="submit">Set</button>
    </form>
  </div>
</template>

<script>
export default {
  //state
  data() {
    return {
      count: 0,
      submittedCount: '',
    }
  },

  //actions
  methods: {
    increment() {
      this.count++
    },
    decrement() {
      this.count--
    },
    reset() {
      this.count = 0
    },
    submitForm() {
      if (!this.submittedCount) {
        alert('Please enter number to input field')
        return
      }

      this.count = this.submittedCount
      // alert(`${this.submittedCount} has been set`)
      this.submittedCount = ''
    },
  },
}
</script>

<style>
.increment-button {
  margin-right: 1rem;
}
.decrement-button {
  margin-right: 1rem;
}

.buttons-div {
  margin-top: 2rem;
}

.counter-div {
  margin-top: 5rem;
  text-align: center;
}

.input-div {
  margin-top: 1rem;
}
</style>
