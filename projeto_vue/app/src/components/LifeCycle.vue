<template>
    <div>
        <h1>Meu nome é : {{ nome }}</h1>
        
    </div>
</template>

<script>
export default {
    name: 'LifeCycle',
    data(){
        return{
            nome: "ainda não sei"
        }
    },
    created(){
        setTimeout(()=> {
            this.nome = "Ruan" 
        }, 3000)
        this.lifeCycle()
    },
    
    mounted(){
        setTimeout(()=> {
            this.nome = "Pedro" 
        }, 2000)
    },
    methods:{
        lifeCycle(){
            console.log("executou");
        }
        
    }

}

</script>

