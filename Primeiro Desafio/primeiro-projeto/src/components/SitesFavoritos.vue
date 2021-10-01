<template>
    <div class ="Sites-Favoritos">
        <h2>Sites Favoritos</h2>
        <ul>
            <li v-for="id of sites" v-bind:key="id">
                <a v-bind:href="id.url">{{id.nome}}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'SitesFavoritos',

    data() {
        return {
            sites: [
                /**{
                  id:1,
                    nome:'Google',
                    url: 'https://www.google.com.br'
                },
                {
                    id:2,
                    nome:'Youtube',
                    url: 'https://www.youtube.com.br'
                },
                {
                    id:3,
                    nome:'GitHub',
                    url:'https://github.com/',
                }*/
            ]
        }
    },
        created() {
            fetch('https://hackthon-decola.firebaseio.com/sites-favoritos.json')
                .then(resultado => resultado.json())
                .then(json => {
                    this.sites = json;
                });
        }
}
</script>

<style scoped>

</style>