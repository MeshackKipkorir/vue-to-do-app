<template>
  <div>
    <h2>To do list</h2>
    <ul>
      <li v-bind:key="todo.id" v-for="todo in todos">
        <Todo v-bind:todo="todo"/>
      </li>
    </ul>

  </div>
</template>

<script>
  import Todo from './Todo'

  export default{
    name:'Todo_list',
    components: {
      Todo
    },
    props:[
    "todos"
    ]
  }
</script>
