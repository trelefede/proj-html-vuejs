<template>
    <div class="ft-bg-blue" id="height">
        <div class="container">

            <!-- heading section  -->
            <div class="row pt-4">
                <div class="col-12 text-center">
                    <p class="mt-4 mb-2 ft-color-red">Price List</p>
                    <h3 class="fw-light fs-1 mb-3"><span class="fw-bold">Our</span> Pricing</h3>
                    <p>When, while the lovely valley teems with vapour around meand the meridian sun strikes <br> the upper surface .</p>
                </div>
            </div>

            <!-- content section create by data.js-->
            <div class="row">
                <PriceListCardComponent class="col-4" v-for="cardData in priceListData" :key="cardData.title" :cards="cardData" />
            </div>
        </div>
    </div>
</template>


<script>
import PriceListCardComponent from "@/components/PriceListCardComponent.vue"

import { priceListData } from "@/data/data.js"

export default {
    name: "PriceListComponent",
    data(){
        return {
            priceListData
        }
    },
    components: {
        PriceListCardComponent
    },
}
</script>


<style lang="scss" scoped>
#height{
    height: 600px;
}

p{
    font-size: 0.9rem;
}
</style>