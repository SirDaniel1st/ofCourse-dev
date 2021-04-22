<template>
  <div id="app">
    <span class="bg">
      <img class= "logo" alt="ofCourse logo" src="./assets/logo.png" >
      <HelloWorld msg="Rate Your Courses"/>

      
    </span>
  </div>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #4fc0b8;
  font-size: 30.3px;
  margin-top: 100px;
}
.bg {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background: url( 'https://i.ibb.co/X2x1XpX/background.png') no-repeat center center;
    background-size: cover;
    background-color: red;
    transform: scale(1.1);
  }

.logo{
  margin-top: 150px;
  height: 250px;
  width: 600px;
}
</style>
