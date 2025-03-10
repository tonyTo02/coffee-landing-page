<template>
    <div class="container flex flex-row w-full items-center px-[10%] py-12">
        <div class="image w-12">
            <img :src="logoPage" alt="logo" srcset="">
        </div>
        <div class="title w-1/2 px-2">
            <p class="font-bold text-2xl text-[#2F2105]">CoffeeLove</p>
        </div>
        <div class="md:social-media md:grow md:justify-items-center hidden">
            <div class="wrap flex flex-row">
                <img class="p-3" :src="facebookIcon" alt="facebook">
                <img class="p-3" :src="instagramIcon" alt="instagram">
                <img class="p-3" :src="twitterIcon" alt="twitter">
            </div>
        </div>
    </div>
    <div class="flex md:flex-row items-center md:px-[15%] md:pb-20 flex-col">
        <div class="navigation text-[#835E4C] w-[80%]">
            <p class="py-1.5">HOME</p>
            <p class="py-1.5">MENU</p>
            <p class="py-1.5">DELIVERY</p>
            <p class="py-1.5">LOCATIONS</p>
        </div>
        <div class="subscribe w-[80%] mt-2">
            <label for="email" class="font-bold text-2xl text-[#2F2105]">Newsletter</label>
            <div class="wrap flex flex-row pt-4 items-center">
                <input type="text" name="email" id="email" class="bg-[#F6EBDA] text-[#835E4C] p-4"
                    placeholder="Your Email">
                <button class="bg-[#835E4C] w-30 p-4 text-center text-white">Subscribe</button>
            </div>
        </div>
        <div class="social-media grow justify-items-center py-10 md:hidden">
            <div class="wrap flex flex-row">
                <img class="p-3" :src="facebookIcon" alt="facebook">
                <img class="p-3" :src="instagramIcon" alt="instagram">
                <img class="p-3" :src="twitterIcon" alt="twitter">
            </div>
        </div>
    </div>
</template>

<script>
import IconSocial1 from '@/assets/images/facebook_logo.png';
import IconSocial2 from '@/assets/images/instagram-logo.png';
import IconSocial3 from '@/assets/images/twitter-logo.png';
import LogoPath from '@/assets/images/CoffeeLove.svg';
export default {
    data() {
        return {
            facebookIcon: IconSocial1,
            instagramIcon: IconSocial2,
            twitterIcon: IconSocial3,
            logoPage: LogoPath,
        }
    }
}
</script>