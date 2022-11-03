<template>
  <h1>Olá mundo {{testando}}</h1>
<primeiroComponete />
</template>

<script>
import primeiroComponete from './components/primeiroComponete.vue';

export default{
  name: 'App',
  components: {
    primeiroComponete
  },
  data(){
  return{
    testando: "teste"
  }
}
}



</script>