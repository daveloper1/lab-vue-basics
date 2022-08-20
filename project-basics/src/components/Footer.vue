<template>
    <div>
        <h1>Esto es un footer</h1>
        <h3>Calculadora: {{ 3 + 3 }}</h3>
        <h2>Prop from App.vue: {{ myNumber }}</h2>
        <h3>Función: {{ returnString() }} </h3>
        <h3>Atributo: {{ project }}</h3>
        <h3 v-if="varIt3 > 2">Iteration 3: Probando v-if</h3>
        <h3 v-else-if="varIt3 == 2">Iteration3: Probando v-else-if</h3>
        <h3 v-else>Iteration 3: Probando v-else</h3>
        <h3>Probando condicional ternario: {{ varIt3 === 2 ? project : returnString() }}</h3>
        <h3 v-show="varIt3 === 2">Probando v-show! Está en el div pero cambia la propiedad de visibilidad</h3>
    </div>
</template>

<script>

export default {
    name: "Footer",
    props: {
        myNumber: Number,
    },

    data() {
        return {
            numb: 8,
            project: "Inicialmente es asi",
            varIt3: 3,
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