<template>
  <ul>
    <li v-for='nummer in lista'>
      {{ nummer }}
    </li>
  </ul>
</template>

<script>
export default {
  name: 'Lista',
  computed: {
    lista() {
      return this.$store.state.lista
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
