<template>
    <div>
        <ReutizacaoTeste />
    <h1>Ola Vue</h1>
<p>Meu nome é {{ nome }} e trabalho como {{ profi }}</p>
<ReutizacaoTeste />
<MultEvents />

<ReutizacaoTeste />
</div>
</template>

<script>
import MultEvents from "./MultEvents.vue";
import ReutizacaoTeste from "./ReutizacaoTeste.vue";

export default{
    name : 'primeiroComponente',
    components: {
        MultEvents,
        ReutizacaoTeste
    },
 
    data(){
        return{
            nome: "Ruan",
            profi: "Desenvolvedor PHP"
        }
    }
}

</script>