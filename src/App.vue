<template>
  <div class="container">
    <h1>Chuck Norris Jokes</h1>
    <ul class="jokes-list">
      <li v-for="(joke, index) in chuck" :key="index" class="joke-item">
        {{ joke.value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      chuck: [
        { value: "Chuck Norris puede saltar en paracaídas al espacio exterior." },
        { value: "El principal producto de Chuck Norris es el dolor." },
        { value: "Chuck Norris no lee libros. Los mira fijamente hasta que obtiene la información que quiere." },
        { value: "El tiempo no espera a nadie. A menos que ese hombre sea Chuck Norris." },
        { value: "Si escribes Chuck Norris en Scrabble, ganas. Para siempre." }
      ]
    };
  }
};
</script>

<style>
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

.container {
  max-width: 800px;
  margin: 50px auto;
  padding: 20px;
  background-color: white;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

h1 {
  color: #333;
  text-align: center;
  border-bottom: 2px solid #eee;
  padding-bottom: 10px;
}

.jokes-list {
  list-style: none;
  padding: 0;
}

.joke-item {
  padding: 15px;
  margin: 10px 0;
  background-color: #f8f8f8;
  border-radius: 5px;
  transition: transform 0.2s;
}

.joke-item:hover {
  transform: translateX(10px);
  background-color: #fff3d4;
}
</style>