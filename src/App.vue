<template>
  <div>
    <Header />
    <p class="titulo">Hildinair Ciência&Tecnologia</p>
    <Pessoa />
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import LiveCycle from './components/LiveCycle.vue'
  import Pessoa from "./components/Pessoa.vue";
  export default {
    name: "App",
    components: {
      Header,
      LiveCycle,
      Pessoa,
    }
  }
</script>

<style>
  body {
    background-color: #0f0f0f;
    color: aliceblue;
  }
  a {
      color:darkgrey;
  }
  .menssage {
    background-color:black;
  }
</style>
