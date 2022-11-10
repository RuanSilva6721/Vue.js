<template>
    <div>
        
 <div>
    <button @click="primeiro($event), segundo($event), terceiro($event)">Ativar multiplos métodos</button>
    <P>{{mult_events}}</P>
 </div>
 
 
    </div>
</template>

<script>
export default {
    name: "MultEvents",
    data(){
        return{
            mult_events: ""
        }
    },
    methods: {
        primeiro(e){
            e.preventDefault();
            this.mult_events = "Primeiro Evento ativado"
        },
        segundo(){
           setTimeout(() => this.mult_events = "Segundo Evento ativado!", 500)
        },
        terceiro(){
           setTimeout(() => this.mult_events = "", 1500)
        }
    }

}


</script>

<style scoped>
div{
    margin: 150px;
}

</style>