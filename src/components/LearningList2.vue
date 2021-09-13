<template>
  <div>
    <h1>{{ header }}</h1>
    <ul>
      <li v-for="(thing, idx) in financial" v-bind:key="idx">{{ thing }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'LearningList2',
  props: {
    header: String,
  },
  data: function() {
    return { 
      financial: [
          "Investing",
          "Bugeting",
          "Balancing a checkbook"
      ],
    } 
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  padding: 0;
  display: inline-block;
}
li {
  color: deeppink;
  margin: 0 10px;
}

</style>
