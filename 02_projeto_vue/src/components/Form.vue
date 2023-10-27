<template>
<div>
    <h2>Meu formulário</h2>
    <form action="">
        <div>
            <InputTex />
        </div>
        <div>
            <InputTex />
        </div>
        <div>
            <Submit />
        </div>
    </form>
    </div>
</template>

<script>
    import InputTex from './form/InputText.vue'
    import Submit from './form/Submit.vue'

    export default {
        name: 'Form',
        components: {
            InputTex,
            Submit        
        }
    }
</script>
