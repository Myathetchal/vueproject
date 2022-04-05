<template>
  <div id="app">
    <TaskList :tasks="tasks"/>
    <TaskItem :tasks="tasks"/>
  </div>
</template>

<script>
import TaskList from './components/TaskList.vue'
import TaskItem from './components/TaskItem.vue'

export default {
  name: 'App',
  components: {
    TaskList, TaskItem
  },
  data () {
    return {
      tasks: [
        {
          title: 'test1',
          completed: false
        },
        {
          title: 'test2',
          completed: false
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
