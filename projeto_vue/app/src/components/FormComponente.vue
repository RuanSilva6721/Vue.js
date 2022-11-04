<template>

    <form action="">
        <!-- <input type="text" name="" id="">
        <input type="text" name="" id="">
        <input type="submit" value="Enviar"> -->
        <div><InputText /></div>
        <div><InputText /></div>
        <div><SubmitForm /></div>

    </form>

</template>
<script>
import InputText from './form/InputText.vue'
import SubmitForm from './form/SubmitForm.vue'


export default{
        name: 'FormComponente',
        components: {
            SubmitForm, 
            InputText
        }
}

</script>