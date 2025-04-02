<template>
  <div class="col-12 col-md-4 mb-4">
    <div class="card h-100 shadow">
      <img 
        :src="icon_url" 
        class="card-img-top"
        alt="Chuck Norris"
      >
      <div class="card-body">
        <p class="card-text">{{ value }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    icon_url: String,
    value: String
  }
};
</script>

<style scoped>
.card {
  transition: transform 0.3s;
}
.card:hover {
  transform: translateY(-5px);
}
</style>