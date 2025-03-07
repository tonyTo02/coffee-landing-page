<template>
    <div class="card w-80 h-118 relative bg-[#835E4C] text-white rounded-3xl shadow-4xl p-5">
        <div class="img w-full flex justify-center">
            <img :src="cardImages" alt="product images">
        </div>
        <div class="title pt-7">
            <p class="text-xl mb-3">{{ cardTitle }}</p>
        </div>
        <div class="content">
            <p>{{ cardContent }}</p>
        </div>
        <div class="footer grid grid-cols-[60%_40%] gap-1 items-center absolute bottom-2">
            <p class="price text-xl">
                ${{ cardPrice }}
            </p>
            <button class="button-order w-32 h-10 rounded-full bg-[#A0583C] ms-6">
                Order now
            </button>
        </div>
    </div>
</template>

<script>
export default {
    props: [
        'cardImages',
        'cardTitle',
        'cardContent',
        'cardPrice',
    ],
}
</script>