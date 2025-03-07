<template>
    <div class="small-card-product relative w-70 h-67 text-white bg-[#835E4C] shadow-xl rounded-2xl items-center p-4">
        <div class="img items-center flex justify-center">
            <img :src="image" alt="{{ name }}" srcset="" class="">
        </div>
        <div class="name text-2xl ps-2 font-bold p-1">
            <p>{{ name }}</p>
        </div>
        <div class="price ps-2 text-xl font-bold p-1">
            <p>${{ price }}</p>
        </div>
        <div class="absolute text-right bottom-4 right-4">
            <button class="w-28 h-10 rounded-3xl shadow-xl bg-[#A0583C]" @click="clickedButton">
                Order now
            </button>
        </div>
    </div>
</template>
<script>

export default {
    props: [
        'image',
        'name',
        'price',
    ],
    methods: {
        clickedButton() {
            this.$emit('order-clicked');
        }
    }
}
</script>