<template>
  <div id="app">
    <Todo_list v-bind:todos="todos" />
  </div>
</template>

<script>

import Todo_list from './components/Todo_list';

export default{
    name:'app',
    components:{
      Todo_list
    },
    data(){
      return{
      todos:[
        {
          id:1,
          title:'Go WorkOut',
          completed:false
        },
        {
          id:2,
          title:'Learn Vue Js',
          completed:true
        },
        {
          id:3,
          title:'Shopping',
          completed:true
        },
        {
          id:4,
          title:'Go play football',
          completed:false
        },
        {
          id:5,
          title:'Do dishes',
          completed:false
        }
      ],
      }
    },
  }
</script>

<style>

</style>
