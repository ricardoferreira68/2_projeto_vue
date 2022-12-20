<template>
  <div>
    <!-- <PrimeiroComponente /> -->
    <!-- <LiveCycle /> -->
    <pessoa />
  </div>
</template>

<script>
  // import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LiveCycle from './components/LiveCycle.vue'
  import Pessoa from "./components/Pessoa.vue";
  export default {
    name: "App",
    components: {
      // PrimeiroComponente,
      LiveCycle,
      Pessoa,
    }
  }
</script>
