<template>
  <div class="about">
    <button v-on:click="clickNow(2, $event)">Click me</button>
    <p v-if="counter == 0">Ingen click lige nu</p>
    <p v-else-if="counter > 0">Likes: {{ counter }}</p>
    <p v-else>Fejl her!</p>
    <input type="text" v-on:keyup.enter="alertMe" />
    <p v-if="InputText == true">Godkendt indhold!</p>
  </div>
</template>


<script>
export default {
  el: "about",
  data: function() {
    return {
      counter: 0,
      InputText: false
    };
  },
  methods: {
    clickNow: function(step) {
      this.counter += step;
    },
    alertMe: function() {
      this.InputText = true;
    }
  }
};
</script>
