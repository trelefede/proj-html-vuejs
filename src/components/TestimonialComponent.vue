<template>
    <div class="container">
        <!-- heading section  -->
        <div class="row">
            <div class="col-12 text-center">
                <p class="mt-4 mb-2 ft-color-red">Testimonial</p>
                <h3 class="fw-light fs-1 mb-3"><span class="fw-bold">What</span> People Say</h3>
                <p id="heading-content">When, while the lovely valley teems with vapour around meand the meridian sun strikes <br> the upper surface .</p>
            </div>
        </div>
        <div class="row">
            <TestimonialCardComponent />
        </div>
    </div>
</template>

<script>
import TestimonialCardComponent from "@/components/TestimonialCardComponent.vue"

export default {
    name: "TestimonialComponent",
    components: { 
        TestimonialCardComponent
    },
}
</script>

<style lang="scss" scoped>

</style>