<template>
<div>
    <h1>Esto es un footer</h1>
    <h3>Calculadora: {{ 3 + 3 }}</h3>
    <h2>Prop from App.vue: {{ myNumber }}</h2>
    <h3>Función: {{ returnString() }} </h3>
    <h3>Atributo: {{ project }}</h3>
    <h1 v-if="2>1">Probando v-if</h1>
    <h1 v-else>Oh nooooo</h1>
</div>
</template>

<script>

export default {
    name:"Footer",
    props: {
        myNumber: Number,
    },

    data() {
        return {
            numb: 8,
            project: " ",
        }
    },

    methods: {
        returnString() {
            return "Hola Mundo";
        }
    },

    created() {
        this.project = 'Hola Mundo de nuevo';
    },

}


</script>

<style>
</style>