<template>
    <div id="app">
        <img src="./src/assets/coffee-house-cafe-logo.png"/>
        <h1>{{ msg }}</h1>
        <button v-on:click="onMachinesListClick">{{msg2}}</button>
        <button v-on:click="onMapClick">{{msg3}}</button>
        <ListMachines> </ListMachines>
        <MapMachines> </MapMachines>
    </div>
</template>

<script>
    export default {
        name: 'app',
        data() {
            return {
                msg: 'Gestion  machines à café',
                msg2: 'Consulter la liste des machines',
                msg3: 'Voir la carte'
            }
        },
        methods: {
            onMachinesListClick: function () {
                alert('Vous avez cliqué sur la liste des machines ')
            },
            onMapClick: function () {
                alert('Vous avez cliqué sur l\'emplacement des machines')
            }
        }
    }
</script>

<style scoped>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }

    h1, h2 {
        font-weight: normal;

    }

    button {
        background-color: #B4AF91;
        padding-left: 10%;
        padding-right: 10%;
        height: 50px;
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        font-size: 120%;

    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>
