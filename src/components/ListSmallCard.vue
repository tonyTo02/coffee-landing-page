<template>
    <div class="container h-screen md:py-5">
        <div class="py-10 ps-4">
            <p class="font-bold text-2xl">Special menu <span class="underline decoration-4 decoration-[#FFBD7F]">for
                    you</span></p>
        </div>
        <div
            class="list-small-card-product ms-40 w-full md:ms-0 grid grid-cols-4 gap-x-[60%] gap-4 md:gap-2 justify-items-center">
            <small-card v-for="(x, index) in listSmallCards" :key="index" v-bind:image="x.image" v-bind:name="x.name"
                v-bind:price="x.price" :class="[, { 'bg-[#FFBD7F]': x.isClicked }]"
                @order-clicked="handleClicked(index)" />
        </div>
    </div>
</template>
<script>
import SmallCard from './SmallCard.vue';
import MenuProduct1 from '@/assets/images/menu_item_1.png';
import MenuProduct2 from '@/assets/images/menu_item_2.png';
import MenuProduct3 from '@/assets/images/menu_item_3.png';
import MenuProduct4 from '@/assets/images/menu_item_4.png';
import MenuProduct5 from '@/assets/images/menu_item_5.png';
import MenuProduct6 from '@/assets/images/menu_item_6.png';
import MenuProduct7 from '@/assets/images/menu_item_7.png';
import MenuProduct8 from '@/assets/images/menu_item_8.png';
export default {
    components: {
        'small-card': SmallCard,
    },
    data() {
        return {
            listSmallCards: [
                { image: MenuProduct1, isClicked: false, name: "Macchiato", price: 8.60 },
                { image: MenuProduct2, isClicked: false, name: "Caramel Frappé", price: 8.20 },
                { image: MenuProduct3, isClicked: false, name: "Macha Latte", price: 11.40 },
                { image: MenuProduct4, isClicked: false, name: "Hot Chocolate", price: 6.40 },
                { image: MenuProduct5, isClicked: false, name: "Fruit Tea", price: 8.60 },
                { image: MenuProduct6, isClicked: false, name: "Cappacino", price: 9.20 },
                { image: MenuProduct7, isClicked: false, name: "Affogato", price: 11.40 },
                { image: MenuProduct8, isClicked: false, name: "Cold Brew", price: 6.40 },
            ],
        }

    },
    methods: {
        handleClicked(index) {
            this.listSmallCards.forEach((item, i) => {
                item.isClicked = i === index;
            });
        }
    }
}
</script>