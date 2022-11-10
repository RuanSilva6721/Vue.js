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


        <p>testando back-end</p>

        <ul>
            <li v-for="(tec, index) in backend_tech" v-bind:key="index">{{tec}}</li>
    <p>a mais</p>
        </ul>


        <p>ultilizo as linguagem front-end</p>
        <ul>
            <li v-for="(tec, index) in front_tech" v-bind:key="index">{{tec.language}}</li>
        </ul>
    </div>


</template>
<script>
export default {
    name: 'PessoaInfo',
    data(){
        return{
        esta_trabalhando: false,
        meu_link: 'https://google.com',
        mostrar_email: true,
        backend_tech: ['Python', 'PHP', 'JavaScript'],
        front_tech: [
            {id: 1, language: 'HTML'}, 
            {id: 2, language: 'CSS'},
            {id: 3, language: 'VUE.JS'},
        ]
        }
    },
    methods:{
            showEmail(){
                this.mostrar_email = !this.mostrar_email;
            }
    }
}

    
</script>
