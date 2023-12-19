<template>
  <header class="main-header">
    <div class="logo">
      <img :src="require('@/assets/logo.png')" alt="Logo" />
    </div>
    <div class="title">
      <h1>{{ pageTitle }}</h1>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      pageTitle: 'Yughioh-api'
    };
  }
};
</script>

<style scoped>
/* Stili per l'header */
.main-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #f3f3f3;
}

/* Stili per il logo */
.logo img {
  width: 60px;
  /* Dimensione del logo */
}

/* Stili per il titolo */
.title h1 {
  margin: 0;
  font-size: 24px;
}
</style>
