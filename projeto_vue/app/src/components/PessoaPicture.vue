<template>
    <div>
        <p>teste</p>
        <img class="imgTamanhp" :src="myavatar" :alt="descricao">
        <MudarImagem @mudar-imagem="mudarImagem" />
    </div>
</template>


<script>import MudarImagem from "./MudarImagem.vue"
export default {
    name: "PessoaPicture",
    data(){
        return{
        myavatar: "/img/cara.webp",
        descricao: "Ruan"
        }
    },
    components: {
        MudarImagem
    },
    methods: {
        mudarImagem(){
            this.myavatar = "/img/teste.jpg"
        }
    }

}
</script>