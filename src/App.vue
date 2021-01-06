<template>
  <div id="app">
    <Header/>
    <div class="main">
      <router-view name="main"></router-view>
    </div>
  </div>
</template>

<script>
import Header from "./components/Header";
import PostList from "./components/PostList";
export default {
  name: 'App',
  components: {PostList, Header}
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
body {
  background-color: #e1e1e1;
}
.main {
  width: 74%;
  margin: 0 auto;
}
</style>
