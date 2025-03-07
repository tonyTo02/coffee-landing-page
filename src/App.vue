<script>
import MainPage from './components/MainPage.vue';
import CatalogPage from '@/components/CatalogComponent.vue';
import ListProductCards from './components/ListProductCards.vue';
import AdvertiseBanner from './components/AdvertiseBanner.vue';
import ListSmallCard from './components/ListSmallCard.vue';
import AboutUs from './components/AboutUs.vue';
import FooterPage from './components/FooterPage.vue';
export default {
    components: {
        'main-page': MainPage,
        'catalog-page': CatalogPage,
        'list-cards': ListProductCards,
        'ads-banner': AdvertiseBanner,
        'list-small-cards': ListSmallCard,
        'about-us': AboutUs,
        'footer-page': FooterPage,
    }
}
</script>

<template>
    <div class="relative">
        <main-page></main-page>
        <catalog-page class="absolute bottom-[-8%]" />
    </div>
    <list-cards></list-cards>
    <ads-banner />
    <list-small-cards />
    <about-us />
    <footer-page></footer-page>
</template>

<style scoped></style>
