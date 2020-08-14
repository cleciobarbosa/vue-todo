<template>
  <div id="app" class="container">
    <img alt="Vue logo" class="logo" src="./assets/logo.png" />
    <todo-list></todo-list>
  </div>
</template>
<script>
import TodoList from "./components/TodoList.vue";
export default {
  name: "App",
  components: {
    TodoList
  }
};
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}
.container {
  max-width: 600px;
  margin: 0 auto;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
}

.logo {
  display: block;
  margin: 20px auto;
  height: 75px;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
