<template>
    <nav class="container">
        <select v-model="selectedArchetype" class="search-bar" @change="updateSearch">
            <option value="">All</option>
            <option v-for="archetype in archetypes" :value="archetype.archetype_name" :key="archetype.id">
                {{ archetype.archetype_name }}
            </option>
        </select>
    </nav>
</template>
  
<script>
export default {
    data() {
        return {
            selectedArchetype: '',
            archetypes: [
                { id: 1, archetype_name: 'Archetype 1' },
                { id: 2, archetype_name: 'Archetype 2' },

            ]
        };
    },
    methods: {
        updateSearch() {
            this.$emit('search', this.selectedArchetype);
        }
    }
};
</script>
  
<style scoped lang="scss">
@import "../assets/scss/utils.scss";

.search-bar {
    width: 9.375rem;
    height: 2.5rem;
    margin: 1.5625rem 0 1.5625rem .625rem;
}
</style>
  