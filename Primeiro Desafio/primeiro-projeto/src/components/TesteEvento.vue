<template>
    <div class="Teste-Evento">
        <h2>Teste Evento</h2>
        <p v-on:click="deixarMaiuscula">{{ mensagem }}</p>
    <!-- O V-on: pode ser substituido por @ -->
    </div>
</template>

<script>
export default {
    data(){
        return{
            mensagem: 'O rato roeu a roupa do rei de Roma'
        }
    },
    methods:{
        deixarMaiuscula(){
            this.mensagem = this.mensagem.toUpperCase();
        }
    }
}
</script>

<style scoped>

    #Teste-Evento{
        background-color: burlywood;
    }
</style>