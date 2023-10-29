<template>
    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro()">Ativar múltiplos eventos</button>
        <p>{{ multiplos_eventos}}</p>
    </div>
</template>

<script>
    export default {
        name: 'MultiplosEventos',
        data(){
            return {
                multiplos_eventos: "",
                txt1: "Primeiro Evento",
                txt2: "Segundo Eventoooo"
            }
        },
        methods: {
            primeiro(txt, e) {
                this.multiplos_eventos = txt;
            },
            segundo(txt, e) {
                setTimeout(() => {
                    this.multiplos_eventos = txt;
                }, 2500);
            },
            terceiro(){
                 setTimeout(() => {
                    this.multiplos_eventos = "";
                }, 5000);
            }
        }
    }
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>