<template>
  <div>
    <header>
      <h1>Header</h1>

    </header>

    <div class="container">
      <h2>Container</h2>
      <div class="grid">

        <div v-for="card in cards" :key="card.id" class="card">

          {{ card.title }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cards: []
    };
  },
  mounted() {

  },
  methods: {

  }
};
</script>

<style scoped>
header {
  background-color: #333;
  color: white;
  padding: 20px;
}

.container {
  width: 80%;
  margin: 20px auto;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

.card {
  border: 1px solid #ccc;
  padding: 10px;

}
</style>
