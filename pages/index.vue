<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <h2>Carousel</h2>
      <v-carousel>
        <v-carousel-item v-for="(item,i) in items" :src="item.src" :key="i"></v-carousel-item>
      </v-carousel>

      <h2>Card Media</h2>
      <v-card>
        <v-card-media src="https://dummyimage.com/600x400/de33de/fff" height="600px"></v-card-media>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  data () {
    return {
      items: [
        { src: 'https://dummyimage.com/600x400/000/fff' },
        { src: 'https://dummyimage.com/600x400/fff/000' }
      ]
    }
  }
}
</script>
