<template>
    <div class="teste-for">
        <h2>Teste For</h2>
        <ul>
            <li v-for="fotos of gatos" v-bind:key="fotos.id">
                <img v-bind:src="fotos.url" v-bind:alt="fotos.nome">
            </li>
            <!--No caso do v-bind:'qualquer coisa', podemos usar apenas o :-->
            <!--<li>
                <img src="https://ervadegato.com.br/blog/wp-content/uploads/2021/08/maine-coon-maior-gato-2.jpg" alt="">
            </li>
            <li>
                <img src="https://mega.ibxk.com.br/2016/08/23/23184723908456.jpg?ims=610x" alt="">
            </li>-->
        </ul>
    </div>
</template>

<script>
export default {
    name: 'TesteFor',
    data() {
        return{
            gatos: [
                {
                    id: 1,
                    nome: 'Gato Cinza',
                    url: 'https://ervadegato.com.br/blog/wp-content/uploads/2021/08/maine-coon-maior-gato-2.jpg'
                },
                {
                    id: 2,
                    nome: 'Gato Branco',
                    url: 'https://mega.ibxk.com.br/2016/08/23/23184723908456.jpg?ims=610x'
                }
            ]
        }
    }
}
</script>

<style scoped>
    img{
        width:30vw
}
</style>