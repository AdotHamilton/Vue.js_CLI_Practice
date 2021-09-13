<template>
  <div>
    <h1>Austin's learning lists</h1>
    <learning-list header="Tech" />
    <learning-list-2 header="Finance"/>
  </div>
</template>

<script>
import LearningList from './components/LearningList.vue'
import LearningList2 from './components/LearningList2.vue'

export default {
  name: 'App',
  components: {
    LearningList,
    LearningList2
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
