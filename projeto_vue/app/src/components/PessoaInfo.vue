<template>
    <div>
       <p>nome é Felipe</p> 
        <p v-if="esta_trabalhando">Estou trabalhando</p>
        <p v-else> estou desempregado</p>


        <p>para acessar meu portifólio <a v-bind:href="meu_link">Basta clicar aqui</a></p>
        <div>
            <button @click="showEmail">Mostrar e-mail</button>
        </div>
        <p v-show="mostrar_email">meu e-mail é teste@email.com</p>
    </div>
</template>
<script>
export default {
    name: 'PessoaInfo',
    data(){
        return{
        esta_trabalhando: false,
        meu_link: 'https://google.com',
        mostrar_email: true
        }
    },
    methods:{
            showEmail(){
                this.mostrar_email = !this.mostrar_email;
            }
    }
}

    
</script>
