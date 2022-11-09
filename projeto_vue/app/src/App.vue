<template>
<HeaderComp />

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
import HeaderComp from './components/HeaderComp.vue'

export default{
  name: 'App',
  components: {
    primeiroComponete,
    LifeCycle,
    PessoaTeste,
    PessoaPicture,
    HeaderComp

  },
  data(){
  return{
    testando: "teste"
  }
}
}



</script>

<style>
body{
    background-color: #333;
    color:#fff
}

a {
    color: red;
}
.imgTamanhp{
    height: 250px;
}
</style>