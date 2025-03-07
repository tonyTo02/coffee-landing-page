<template>
    <div class="container flex flex-row justify-center w-full h-132 bg-[#F6EBDA] p-15 items-center">
        <div class="image p-2 rounded-2xl mx-4 bg-white w-full shadow-xl">
            <img :src="image" class="rounded-2xl w-full" alt="image-about-us">
        </div>
        <div class="content px-30">
            <p class="text-2xl font-bold py-5">About <span class="underline decoration-3 decoration-[#FFBD7F]">Us</span>
            </p>
            <p class="text-xl font-bold py-5">Sip into Perfection</p>
            <p class="py-5">Our Coffee World, where passion meets percision in every brew, bring you a symphony of
                flavors and a
                journey through the rich, aromatic realms of coffee craftsmanship.</p>
            <button class="bg-[#2F2105] font-bold text-[#FFBD7F] h-12 w-40 rounded-full">Start our Order</button>
        </div>
    </div>
</template>
<script>
import ImagePath from '@/assets/images/waiter.png';
export default {
    data() {
        return {
            image: ImagePath,
        }
    }
}
</script>