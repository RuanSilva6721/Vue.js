<template>
    <div>
    <h1>Ola Vue</h1>
<p>Meu nome é {{ nome }} e trabalho como {{ profi }}</p>

<MultEvents />
</div>
</template>

<script>
import MultEvents from "./MultEvents.vue"

export default{
    name : 'primeiroComponente',
    components: {
        MultEvents
    },
 
    data(){
        return{
            nome: "Ruan",
            profi: "Desenvolvedor PHP"
        }
    }
}

</script>