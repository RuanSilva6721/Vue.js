<template>
  <h1>Olá mundo {{testando}}</h1>
<primeiroComponete />

<LifeCycle />

<PessoaTeste />
</template>

<script>
import primeiroComponete from './components/primeiroComponete.vue'
import LifeCycle from './components/LifeCycle.vue'
import PessoaTeste from './components/PessoaTeste.vue'


export default{
  name: 'App',
  components: {
    primeiroComponete,
    LifeCycle,
    PessoaTeste
  },
  data(){
  return{
    testando: "teste"
  }
}
}



</script>