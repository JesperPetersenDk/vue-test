<template>
  <div class="about">
    <button v-on:click="clickNow">Click me</button>
    <p>{{ counter }}</p>
  </div>
</template>


<script>
export default {
  el: "about",
  data: function() {
    return {
      counter: 0
    };
  },
  methods: {
    clickNow: function() {
      this.counter++;
    }
  }
};
</script>
