<template>
    <div class="banner w-full h-30 bg-[#F6EBDA] grid grid-cols-[5%_95%] items-center justify-center px-[10%] mt-[5%]">
        <div class="logo size-12">
            <img :src="logo" alt="star-icon">
        </div>
        <div class="content md:px-[5%] md:ms-0 ms-10">
            <p class="text-2xl font-bold">Sign Up to our coffee reward program!</p>
            <p class="text-base font-bold">Learn more &rightarrow;</p>
        </div>
    </div>
</template>

<script>
import logoPath from "@/assets/images/star-icon.png";
export default {
    data() {
        return {
            logo: logoPath,
        }
    }
}

</script>