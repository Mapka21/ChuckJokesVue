<template>
  <div class="container py-5">
    <h1 class="text-center mb-5">Chuck Norris Jokes</h1>
    <div class="row">
      <ChuckCard
        v-for="(joke, index) in chuck"
        :key="index"
        :icon_url="joke.icon_url"
        :value="joke.value"
      />
    </div>
  </div>
</template>

<script>
import ChuckCard from './components/ChuckCard.vue';

export default {
  components: { ChuckCard },
  data() {
    return {
      chuck: [
        {
          icon_url: "https://i.imgur.com/1a9J8TC.png",
          value: "Chuck Norris puede saltar en paracaídas al espacio exterior."
        },
        {
          icon_url: "https://i.imgur.com/1a9J8TC.png",
          value: "El principal producto de Chuck Norris es el dolor."
        },
        {
          icon_url: "https://i.imgur.com/1a9J8TC.png",
          value: "Chuck Norris no lee libros. Los mira fijamente hasta que obtiene la información que quiere."
        },
        {
          icon_url: "https://i.imgur.com/1a9J8TC.png",
          value: "El tiempo no espera a nadie. A menos que ese hombre sea Chuck Norris."
        },
        {
          icon_url: "https://i.imgur.com/1a9J8TC.png",
          value: "Si escribes Chuck Norris en Scrabble, ganas. Para siempre."
        }
      ]
    };
  }
};
</script>