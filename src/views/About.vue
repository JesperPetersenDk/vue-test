<template>
  <div class="about">
    <button v-on:click="clickNow">Click me</button>
    <p v-if="counter == 0">Ingen click lige nu</p>
    <p v-else-if="counter > 0">Likes: {{ counter }}</p>
    <p v-else>Fejl her!</p>
  </div>
</template>


<script>
export default {
  el: "about",
  data: function() {
    return {
      counter: 0,
      x: 0,
      y: 0
    };
  },
  methods: {
    clickNow: function() {
      this.counter++;
    }
  }
};
</script>
