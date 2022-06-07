<template>
  <div id="app">
    <h1>To-Do List</h1>
    <ul>
    <li>
      <to-do-item label="My ToDo Item"></to-do-item>
    </li>
  </ul>
  <h1>Here is a child component!</h1>
  <ButtonCounter />
  </div>
</template>

<script>
  import ToDoItem from './components/ToDoItem.vue';
  // from https://vuejs.org/guide/essentials/component-basics.html#using-a-component
  import ButtonCounter from './components/ButtonCounter.vue'

  export default {
  name: 'app',
  components: {
    ToDoItem,
    ButtonCounter
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>