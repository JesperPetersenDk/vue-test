<template>
  <div class="home">
    {{ title }} 
    <h3>{{ deck }}</h3>
  </div>
</template>

<script>
export default {
  el: "home",
  data: function() {
    return {
      title: "Test Vue js!",
      deck: "Jesper"
    };
  }
};
</script>
