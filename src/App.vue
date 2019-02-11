<template>
  <div id="app" class="container">
    <img src="./assets/logo.png" class="logo">
    <p> <span class="sen-1">Active button displays undone items</span>
    <span class="sen-2">Completed button displays done items</span>
     <span class="sen-3">All button dispaly all items, done/undone</span></p>
    <todo-list></todo-list>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import todoList from './components/todoList'

export default {
  name: 'App',
  components: {
    HelloWorld,
    todoList,
  }
}
</script>

<style>

*{
  box-sizing:border-box;
}
.container{
  max-width:600px;
  margin:0 auto;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 50px;
  /* margin-bottom:33px; */
  font-size:24px;
}
.logo{
  display:block;
  margin:20px auto;
  height: 75px;
}

.sen-1, .sen-2, .sen-3{
  font-size:11px;
  color: #039783;
  text-align:right;
}
</style>
