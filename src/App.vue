<template>
  <div id="app">
    <AppNavbar />
    <HomePage />
    <h1>Welcome to Vue.js</h1>
    <p>This is my first Vue,js App</p>
    <MyComponent />
  </div>
 <img alt="Vue logo" src="./assets/logo.png">
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import MyComponent from './components/MyComponent.vue'
import AppNavbar from './components/AppNavbar.vue'
import HomePage from './views/HomePage.vue'

export default {
  name: 'App',
  components: {
    MyComponent,
    AppNavbar,
    HomePage
  }
  // components: {
  //   HelloWorld
  // }
}
</script>

<style>
#app {
  /** 这是一个字体 */
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased; 
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* 这是一个颜色 */
  color: #2c3e50;  
  /* 这是一个边距 */
  margin-top: 60px; 
}
</style>
