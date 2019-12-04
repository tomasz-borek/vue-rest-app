<template>
  <div id="app">
    <NavigationBar/>
    <img alt="Vue logo" src="./assets/logo.png" />
    <main>
      <ApiPage/>
    </main>
  </div>
</template>

<script>
import HomePage from "./components/HomePage.vue";
import NavigationBar from "./components/NavigationBar.vue";
import SingleComment from "./components/SingleComment.vue";
import ApiPage from "./components/ApiPage.vue";

export default {
  name: "app",
  components: {
    HomePage,
    NavigationBar,
    SingleComment,
    ApiPage
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
