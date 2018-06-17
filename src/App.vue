<template>
  <div id="app">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Title />
    <div class="second">
      <Aside />
      <Content />
    </div>
  </div>
</template>

<script>
  // import HelloWorld from './components/HelloWorld.vue'
  import Title from './components/Title.vue'
  import Aside from './components/Aside.vue'
  import Content from './components/Content.vue'

  export default {
    name: 'app',
    components: {
      Title,
      Aside,
      Content
    }
  }
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700,900');


  html,
  body {
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
    font-family: 'Roboto', serif;

  }

  * {
    box-sizing: border-box;
    position: relative;
    // border: 1px solid black;
  }
  #app{
    width: 100%;
    height: 100%;
    background-color: #F2F2F2;
  }
  .second{
    display: flex;
  }
</style>