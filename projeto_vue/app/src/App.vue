<template>
  <h1>Olá mundo {{testando}}</h1>
<primeiroComponete />

<LifeCycle />

<PessoaTeste />
<PessoaPicture />
</template>

<script>
import primeiroComponete from './components/primeiroComponete.vue'
import LifeCycle from './components/LifeCycle.vue'
import PessoaTeste from './components/PessoaTeste.vue'
import PessoaPicture from './components/PessoaPicture.vue'


export default{
  name: 'App',
  components: {
    primeiroComponete,
    LifeCycle,
    PessoaTeste,
    PessoaPicture

  },
  data(){
  return{
    testando: "teste"
  }
}
}



</script>