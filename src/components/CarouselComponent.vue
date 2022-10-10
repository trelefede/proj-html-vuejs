<template>
    <div id="carousel" class="d-flex">
        <CarouselCardComponent class="" v-for="card in carouselData" :key="card.id" :card="card" />
    </div>
</template>

<script>
import CarouselCardComponent from "@/components/CarouselCardComponent.vue"

import { carouselData } from "@/data/data.js"

export default {
    name: "PortfolioComponent",
    data(){
        return {
            carouselData
        }
    },
    components:{
        CarouselCardComponent
    },
}
</script>

<style lang="scss" scoped>
#carousel{
    margin-top: 4rem;
}
</style>