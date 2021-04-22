<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <input class= "Search" type="text" v-model="search" placeholder="Course Code / Professor's Name"/>
  </div>
  <div>
        <button class=signin onclick='focusMethod'>Sign In</button>
        <button class=signin autofocus>Sign Up</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .Search{
    font-size: 16px;
    font-size: max(16px, 1em);
    font-family: inherit;
    padding: 0.25em 0.5em;
    background-color: #8a8a8a;
    width: 750px;
    margin-top: 15px;
    border-radius: 15px;
  }
  ::placeholder{
    text-align: center;
  }
  .signin{
    color: #4fc0b8;
    border: 5px solid black;
    height: 70px;
    width: 200px;
    font-size: 30px;
    font-family: inherit;
    background-color: transparent;
    border-color: #4fc0b8;
    border-radius: 10px;
    margin-top: 2em;
    margin-left: 2em;
    margin-right: 2em;
  }
</style>