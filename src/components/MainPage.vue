<template>
    <div class="w-full md:h-screen md:relative relative">
        <div class="md:grid md:grid-cols-3 grid grid-cols-2">
            <div class="md:absolute md:w-full mt-6 absolute w-full">
                <navigation-bar />
            </div>
            <div class="md:hidden h-90 bg-white">
            </div>
            <div class="md:hidden h-90 bg-[#FFBD7F]">
            </div>
            <div
                class="col-span-2 h-80 p-12 md:col-span-2 md:bg-[#fff] md:h-screen md:flex md:flex-col md:justify-center md:items-center md:pe-20">
                <div>
                    <p class="text-4xl mb-2 p-2 font-bold">The <b class="font-bold text-[#FFBD7F]">coffee</b> you
                        will <br>
                        fall
                        in
                        <b class="font-bold text-[#FFBD7F]">love</b> with
                    </p>
                    <p class="mb-2 p-2">Sip, savor, and spread the love - where <br> every cup is a caffeinated hug at
                        our cozy <br> coffee heaven!
                    </p>
                    <button
                        class="w-36 h-10 p-2 rounded-full bg-[#2F2105] text-base text-[#fff] active:bg-[#835E4C] transition-colors">
                        Order now
                    </button>
                </div>
            </div>
            <div class="md:bg-[#FFBD7F] md:h-screen md:z-[-1]">
                <img :src="backgroundImage" class="hidden md:absolute md:right-0 md:top-0 md:block">
            </div>
            <div class="md:absolute md:w-90 md:top-[30%] md:left-[60%] absolute w-50 left-[30%] top-20">
                <img :src="CupCoffeeImage" class="rounded-full">
            </div>
        </div>
    </div>

</template>

<script>
import NavigationBar from './NavigationBar.vue';
import iconPath from '@/assets/images/icons-cart.png';
import backgroundPath from '@/assets/images/hero-coffee-beans.png';
import CupOfCoffeePath from '@/assets/images/cup-of-coffee.png'
export default {
    components: {
        'navigation-bar': NavigationBar,
    },
    data() {
        return {
            icon: iconPath,
            backgroundImage: backgroundPath,
            CupCoffeeImage: CupOfCoffeePath,
        }
    },

}
</script>
<style>
button {
    cursor: pointer;
}
</style>