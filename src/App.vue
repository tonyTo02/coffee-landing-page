<script>
import MainPage from './components/MainPage.vue';
import CatalogPage from '@/components/CatalogComponent.vue';
import ListProductCards from './components/ListProductCards.vue';
export default {
    components: {
        'main-page': MainPage,
        'catalog-page': CatalogPage,
        'list-cards': ListProductCards,
    }
}
</script>

<template>
    <div class="relative">
        <main-page></main-page>
        <catalog-page class="absolute bottom-[-8%]" />
    </div>
    <list-cards></list-cards>
    <catalog-page />
</template>

<style scoped></style>
