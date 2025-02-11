<template>
  <div>
    <Header :esta_logado="true" />
    <PrimeiroComponente />
    <p class="paragrafo-pai">O dado de app é: Teste</p>
    <LifeCycle />
    <Pessoa />
  </div>
  
</template>

<script>
import Header from './components/Header.vue';
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue';


  export default {
    name: 'App', 
      components: {
        Header,
        PrimeiroComponente,
        LifeCycle,
        Pessoa
      }
  }
</script>

<style>
body{
  background-color: #333;
  color: #fff;
}

a{
  color: red;
}
.teste{
  background-color: black;
}
</style>