<template>
    <div class="navigation w-full flex flex-row justify-center px-[10%] z-30">
        <p class="w-1/4 align-middle flex justify-center">
            <img class="size-12" :src="logo" alt="Logo">
        </p>
        <div class="w-2/4 grow justify-center flex">
            <p class="w-24 text-right content-center text-[#FFBD7F]">Home</p>
            <p class="w-24 text-right content-center">Menu</p>
            <p class="w-24 text-right content-center">Delivery</p>
        </div>
        <div class="w-64 content-center bg-white flex flex-row rounded-full border-w-1 justify-center items-center p-2 ms-2 focus:outline-2 focus:outline-black focus:outline-offset-2"
            tabindex="0">
            <label for="search-bar" class="form-label sizre-6 content-center">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                    stroke="currentColor" class="size-5">
                    <path stroke-linecap="round" stroke-linejoin="round"
                        d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z" />
                </svg>

            </label>
            <input type="text" name="search-bar" id="search-bar" placeholder="Cold Brew"
                class="w-3/4 focus:outline-none ms-3">
        </div>
        <p class="w-24 text-right content-center ms-3">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                stroke="currentColor" class="size-6">
                <path stroke-linecap="round" stroke-linejoin="round"
                    d="M2.25 3h1.386c.51 0 .955.343 1.087.835l.383 1.437M7.5 14.25a3 3 0 0 0-3 3h15.75m-12.75-3h11.218c1.121-2.3 2.1-4.684 2.924-7.138a60.114 60.114 0 0 0-16.536-1.84M7.5 14.25 5.106 5.272M6 20.25a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Zm12.75 0a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z" />
            </svg>

        </p>
    </div>
</template>
<script>
import logoPath from '@/assets/images/CoffeeLove.svg';

export default {
    data() {
        return {
            logo: logoPath,
        }
    }
}   
</script>
<style scoped>
p {
    cursor: pointer;
}
</style>