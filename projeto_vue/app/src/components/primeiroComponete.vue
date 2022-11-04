<template>
    <div>
    <h1>Ola Vue</h1>
<p>Meu nome é {{ nome }} e trabalho como {{ profi }}</p>
</div>
</template>

<script>
export default{
    name : 'primeiroComponente',
 
    data(){
        return{
            nome: "Ruan",
            profi: "Desenvolvedor PHP"
        }
    }
}

</script>