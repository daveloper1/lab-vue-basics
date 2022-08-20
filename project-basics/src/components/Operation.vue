<template>
  <div>
    <h1>Iteration 4</h1>
    <div class="iteration" v-for="post in posts" :key="post.id">
      <span>id: {{ post.id }},</span>
      <span>title: {{ post.title }},</span>
      <span>description: {{ post.description }},</span>
      <span>content: {{ post.content }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Operation",
  data() {
    return {
      posts: [{
        id: 0,
        title: 'El nombre del viento',
        description: 'Un asesino de reyes',
        content: 'A la espera de Las puertas de piedra',
      },
      {
        id: 1,
        title: 'Canción de hielo y fuego',
        description: 'Muertes inesperadas',
        content: 'A la espera del último libro',
      },
      {
        id: 2,
        title: 'La historia interminable',
        description: 'Parecido a este verano',
        content: 'No está nada mal en verdad',
      }]
    }
  },
}
</script>

<style>
</style>