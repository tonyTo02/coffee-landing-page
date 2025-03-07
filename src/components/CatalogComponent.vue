<template>
    <div class="w-3/4 h-30 flex flex-row justify-center bg-[#F6EBDA] rounded-full px[10%] mx-[15%] p-3">
        <div class="w-1/4 flex flex-col justify-center text-center items-center">
            <img :src="iconHotCoffee" class="w-12 mb-2">
            <p>Hot Coffee</p>
        </div>
        <div class="w-1/4 flex flex-col justify-center text-center items-center">
            <img :src="iconColdCoffee" class="w-12 mb-2">
            <p>Cold Coffee</p>
        </div>
        <div class="w-1/4 flex flex-col justify-center text-center items-center">
            <img :src="iconTea" class="w-12 mb-2 ms-1">
            <p>Tea</p>
        </div>
        <div class="w-1/4 flex flex-col justify-center text-center items-center">
            <img :src="iconDessertCoffee" class="w-12 mb-2">
            <p>Dessert</p>
        </div>
    </div>
    <p>Cold Coffee</p>
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
        }
    }
}
</script>