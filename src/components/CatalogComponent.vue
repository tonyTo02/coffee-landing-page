<template>
    <div
        class="w-full h-70 p-12 gap-2 grid grid-cols-2 bg-[#F6EBDA] items-center justify-items-center md:w-3/4 md:h-30 md:flex md:flex-row md:justify-center md:bg-[#F6EBDA] md:rounded-4xl md:px[10%] md:mx-[15%] md:p-3">
        <div class="w-1/4 flex flex-col justify-center text-center items-center">
            <img :src="iconHotCoffee" class="w-12 mb-2">
            <p>Hot Coffee</p>
        </div>
        <div class="w-1/4 flex flex-col justify-center text-center items-center">
            <img :src="iconColdCoffee" class="w-12 mb-2">
            <p>Cold Coffee</p>
        </div>
        <div class="w-1/4 flex flex-col justify-center text-center items-center">
            <img :src="iconTea" class="w-12 mb-2">
            <p>Tea</p>
        </div>
        <div class="w-1/4 flex flex-col justify-center text-center items-center">
            <img :src="iconDessertCoffee" class="w-12 mb-2">
            <p>Dessert</p>
        </div>
    </div>
</template>
<script>
import HotCoffeePath from "@/assets/images/hot-coffee.png";
import ColdCoffeePath from "@/assets/images/cold-coffee.png";
import TeaPath from "@/assets/images/tea.png";
import DessertPath from "@/assets/images/dessert.png";
export default {
    data() {
        return {
            iconHotCoffee: HotCoffeePath,
            iconDessertCoffee: DessertPath,
            iconColdCoffee: ColdCoffeePath,
            iconTea: TeaPath,
            headingTitle: "Cold Coffee",
        }
    }
}
</script>