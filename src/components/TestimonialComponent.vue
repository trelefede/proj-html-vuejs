<template>
    <div class="container">

        <!-- HEADING SECTION  -->
        <div class="row">
            <div class="col-12 text-center">
                <p class="mt-4 mb-2 ft-color-red">Testimonial</p>
                <h3 class="fw-light fs-1 mb-3"><span class="fw-bold">What</span> People Say</h3>
                <p id="heading-content">When, while the lovely valley teems with vapour around meand the meridian sun strikes <br> the upper surface .</p>
            </div>
        </div>

        <!-- CONTENT SECTION -->
        <div class="row">

            <!-- cards component -->
            <TestimonialCardComponent class="col-4" v-for="card in testimonialData" :key="card.id" :card="card" />
        </div>
    </div>
</template>

<script>
import TestimonialCardComponent from "@/components/TestimonialCardComponent.vue"

import { testimonialData } from "@/data/data.js"

export default {
    name: "TestimonialComponent",
    data(){
        return {
            testimonialData
        }
    },
    components: { 
        TestimonialCardComponent
    },
}
</script>

<style lang="scss" scoped>

</style>