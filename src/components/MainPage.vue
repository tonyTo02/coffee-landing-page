<template>
    <div class="w-full h-screen relative">
        <div class="grid grid-cols-3">
            <div class="absolute  w-full mt-6">
                <navigation-bar />
            </div>
            <div class="col-span-2 bg-[#fff] h-screen flex flex-col justify-center items-center pe-20">
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
                    <button class="w-36 h-10 p-2 rounded-full bg-[#2F2105] text-base text-[#fff] active:bg-[#835E4C]">
                        Order now
                    </button>
                </div>
            </div>
            <div class="bg-[#FFBD7F] h-screen z-[-1]">
                <img :src="backgroundImage" class="absolute right-0 top-0">
            </div>
            <div class="absolute w-90 top-[30%] left-[60%]">
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