<template>
    <div>
        <h2>Nome da Pessoa é: {{nome}}</h2>

        <PessoaInfo :compEmail="email" />
        <FormComponente />

    </div>
</template>


<script>
import PessoaInfo from './PessoaInfo.vue'
import FormComponente from './FormComponente.vue'
export default {
    name: 'PessoaTeste',
    components: {
        PessoaInfo,
        FormComponente
    },
    data(){
        return{
            nome: "Lionel",
            email: "Ruan@compTeste2Email"
        }
    }

}
</script>