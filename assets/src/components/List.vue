<template>
  <div id="app">
    <h2>TodoList</h2>
    <form v-on:submit.prevent>
      <input type="text" v-model="newItem">
      <button v-on:click="addItem">Add</button>
    </form>
    <pre>{{ $data }}</pre>
  </div>
</template>

<script>
export default {
  data() {
    return {
      newItem: '',
      todos:[],
      string: [],
    }
  },
  methods: {
    addItem: function() {
      if (this.newItem === '') {
        return
      }
      var todo = {
        item: this.newItem
      }
      console.log(todo)
      this.todos.push(todo)
      this.newItem = ''
    }
  }
}
</script>

<style scoped>
  div {
    color:  red;
  }
</style>
