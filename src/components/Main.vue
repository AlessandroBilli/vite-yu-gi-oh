<template>
    <div>
        <!-- Contenuto principale, inclusa la griglia delle carte -->
        <div class="main-content">
            <!-- Griglia delle carte -->
            <div class="card-grid">
                <!-- Tuo codice per la generazione delle carte -->
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    // Logica del componente Main
};
</script>
  
<style scoped>
/* Stili per il contenuto principale */
.main-content {
    padding: 20px;
}

/* Stili per la griglia delle carte */
.card-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
}
</style>
  