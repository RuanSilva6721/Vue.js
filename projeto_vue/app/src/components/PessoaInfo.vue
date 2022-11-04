<template>
    <div>
       <p>nome é Felipe</p> 
        <p v-if="esta_trabalhando">Estou trabalhando</p>
        <p v-else> estou desempregado</p>
    </div>
</template>
<script>
export default {
    name: 'PessoaInfo',
    data(){
        return{
        esta_trabalhando: false
        }
    }
}

    
</script>
