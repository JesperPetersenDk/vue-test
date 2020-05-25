<template>
  <div class="Test">
    <h2>Test side</h2>
    <button v-on:click="clickNow(1)">Click me</button>
    <p v-if="counter > 0">
      Count: {{ counter > 20 ? "Større end 20" : "mindre end 20" }}
    </p>
  </div>
</template>

<script>
export default {
  el: "Test",
  data: function() {
    return {
      counter: 0
    };
  },
  methods: {
    clickNow: function(step) {
      this.counter += step;
    }
  }
};
</script>
