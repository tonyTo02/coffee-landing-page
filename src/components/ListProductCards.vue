<template>
    <div
        class="md:list-cards md:relative md:w-full md:grid md:grid-cols-4 md:justify-items-center md:items-center md:mt-[12%] ">
        <div class="md:absolute md:top-[-15%] md:left-10">
            <p class="text-3xl font-bold">Cold <u class="underline decoration-5 decoration-[#FFBD7F]">Coffee</u></p>
        </div>
        <product-card v-for="x in listCards" :key="x.title" v-bind:card-images="x.image" v-bind:card-title="x.title"
            v-bind:card-content="x.content" v-bind:card-price="x.price"
            :class="['hover:bg-[#FFBD7F] hover:scale-110 transition-transform duration-500']"></product-card>
        <div class="prev-slide md:absolute md:left-0 md:p-3 hover:scale-110 cursor-pointer
">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                stroke="currentColor" class="size-8 bg-white rounded-full">
                <path stroke-linecap="round" stroke-linejoin="round"
                    d="m11.25 9-3 3m0 0 3 3m-3-3h7.5M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
            </svg>

        </div>
        <div class="next-slide md:absolute md:right-0 md:p-3 hover:scale-y-110">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                stroke="currentColor" class="size-8 bg-white rounded-full hover:scale-110 cursor-pointer
">
                <path stroke-linecap="round" stroke-linejoin="round"
                    d="m12.75 15 3-3m0 0-3-3m3 3h-7.5M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
            </svg>
        </div>
    </div>
</template>
<script>
import ProductCard from './ProductCard.vue';
import MenuItemPath1 from '@/assets/images/menu_item_1.png';
import MenuItemPath2 from '@/assets/images/menu_item_2.png';
import MenuItemPath3 from '@/assets/images/menu_item_3.png';
import MenuItemPath4 from '@/assets/images/menu_item_4.png';
export default {
    components: {
        "product-card": ProductCard,
    }, data() {
        return {
            listCards: [{
                image: MenuItemPath1, title: "Caramel Frappé"
                ,
                content: "A delightful and indulgent icy beverage blending rich coffee, milk, ice, and sweet caramel syrup, creating a smooth and satisfying treat with a perfect harmony of caffeine and sweetness."
                , price: 8.60
            }, {
                image: MenuItemPath2, title: "Macchiato",
                content: "An espresso-based coffee chacracterized by a perfect balance of bold, concentrated espresso and a touch of velvety steamed milk, creating a nuanced and flavorful experience"
                , price: 8.60
            }, {
                image: MenuItemPath3, title: "Affogato",
                content: "Delectable italian beverage featuring a scoop of creamy vanilla gelato or ice scream 'drowned' or 'affogato' in a shot of hot espresso, creating a delightful contrast of temperatures and flavors."
                , price: 11.40
            }, {
                image: MenuItemPath4, title: "Cold Brew",
                content: "Smooth and concentrated coffe beverage crafted by steeping coarsely ground coffee beans in cold water for an extended period, resulting in a refreshing and less acidic brew that can be enjoyed over ice"
                , price: 6.40
            },],
        }
    },
} </script>
