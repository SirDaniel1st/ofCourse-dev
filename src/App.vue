<template>
  <div id="app">
    <span class="bg">
      <img class= "logo" alt="ofCourse logo" src="./assets/logo.png" >
      <HelloWorld msg="Welcome to Your Vue.js App"/>

      <div class="search-wrapper">
        <input type="text" v-model="search" placeholder="COURSE CODE/ PROFESSOR'S NAME"/>
  </div>
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
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
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
  margin-top: 80px;
  height: 280px;
  width: 600px;
}

.search-wrapper {
    position: relative;
    label {
      position: absolute;
      font-size: 12px;
      color: rgba(0,0,0,.50);
      top: 8px;
      left: 12px;
      z-index: -1;
      transition: .15s all ease-in-out;
    }
    input {
      padding: 4px 12px;
      color: rgba(0,0,0,.70);
      border: 1px solid rgba(0,0,0,.12);
      transition: .15s all ease-in-out;
      background: rgba(22, 8, 49, 0.801);
      &:focus {
        outline: none;
        transform: scale(8);
        & + label  {
          font-size: 10px;
          transform: translateY(-24px) translateX(-12px);
        }
      }
      &::-webkit-input-placeholder {
          font-size: 30px;
          color: rgba(131, 131, 131, 0.5);
          font-weight: 100;
      }
    }
  }
</style>
