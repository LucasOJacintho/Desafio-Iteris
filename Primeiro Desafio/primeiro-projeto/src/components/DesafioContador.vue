<template>
    <div class="Desafio-Contador">
        <h2>Contador</h2>
        <p><strong>Contador:{{valor}}</strong></p>
        <button v-on:click="subtrair">-</button>
        <button v-on:click="somar">+</button>
    </div>
</template>

<script>
    
export default {
    name:"DesafioContador",
    data(){
        return{
            valor: 0
        }
    },
    methods:{
        somar(){
            this.valor ++
        },
        subtrair(){
            this.valor --
        }
    }
}
</script>

<style scoped>

</style>