<template>
  <div id="app">
    <h2>addition = {{ counter }}</h2>
    <button v-on:click="riseCounter">like</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      counter: 10
    };
  },
  methods: {
    riseCounter: function() {
      if (this.counter > 0) {
        this.counter--;
      }
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
