<template>

    <form action="" @submit="enviarFormulario($event)">
        <!-- <input type="text" name="" id="">
        <input type="text" name="" id="">
        <input type="submit" value="Enviar"> -->
        <!-- <div><InputText /></div>
        <div><InputText /></div> -->
        <input type="text" v-model="name">
        <input type="text" v-model="email">
        <div><SubmitForm /></div>

    </form>

</template>
<script>

import SubmitForm from './form/SubmitForm.vue'


export default{
        name: 'FormComponente',
        components: {
            SubmitForm
        },
        data(){
            return{
                name: "",
                email: ""

            }
        },
        methods: {
            enviarFormulario(e){
                e.preventDefault();
                const name = this.name;
                const email = this.email;
                
            console.log("formulário enviado com sucesso!");
            console.log("o nome é:" + name + " o email é:" + email);
        }}
}

</script>