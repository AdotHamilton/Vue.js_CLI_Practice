<template>
  <div>
    <h1>{{ header }}</h1>
    <ul>
      <li v-for="(thing, idx) in tech" v-bind:key="idx">{{ thing }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'LearningList',
  props: {
    header: String,
  },
  data: function() {
    return { 
      tech: [
        "Vue.js",
        "css animation",
        "Firebase"
      ],

    } 
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: auto;
}
ul {
  padding: 0;
  display: inline-block;
}
li {
  color: deepskyblue;
  margin: 0 10px;
}

</style>
