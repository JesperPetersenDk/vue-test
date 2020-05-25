<template>
  <div class="home">
    {{ title }}
    <h3>{{ deck }}</h3>
    <a v-bind:href="link">Ordklar</a>
    <p v-html="linkDone"></p>
  </div>
</template>

<script>
export default {
  el: "home",
  data: function() {
    return {
      title: "Test Vue js!",
      deck: "Jesper",
      link: "https://www.ordklar.dk",
      linkDone: '<a href="https://www.ordklar.dk">Ordklar here</a>'
    };
  },
  methods: {
    sayHello: function() {
      return "hello";
    }
  }
};
</script>
