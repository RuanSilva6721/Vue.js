<template>
    <div>
        <p>teste</p>
        <img :src="myavatar" :alt="descricao">
    </div>
</template>


<script>
export default {
    name: "PessoaPicture",
    data(){
        return{
        myavatar: "/img/cara.webp",
        descricao: "Ruan"
        }
    }

}
</script>