<template>
    <div class="start-project ft-bg-blue">
        <div class="container">
            <div class="row align-items-center py-4 d-flex flex-row-reverse">

                <!-- RIGHT PANEL -->
                <div class="col-6">
                    <p class="text-white">Start Your Project</p>
                    <h2 class="fw-bold">Grow Your Business</h2>
                    <h2 class="fw-light">With Our Strategy</h2>
                    <p class="py-4">When, while the lovely valley teems with vapour around <br> meand the meridian sun strikes the upper surface meand <br> the meridian sun strikes the upper surface</p>
                    <!--  user buttons -->
                    <div class="d-flex justify-content-start pt-2">
                        <a class="btn rounded-pill ft-btn ft-bg-light-red me-4" href="#">Try It Now</a>
                        <a class="btn rounded-pill ft-btn ft-bg-light-blue" href="#">Explore More</a>
                    </div>
                </div>

                <!-- LEFT PANEL -->
                <div class="col-6 d-flex justify-content-center position-relative">
                    <img id="nemoodar" class="position-absolute" src="@/assets/images/nemoodar.png" alt="nemoodar">
                    <img src="@/assets/images/men-data.png" alt="men data">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "StartProjectComponent"
}
</script>


<style lang="scss" scoped>
.start-project{
    padding-top: 6rem;
    padding-bottom: 6rem;
}

h2{
    font-size: 3.3rem;
}

p{
    color: #017999e6;
}

img{
    width: 60%;
    z-index: 9999;
}

#nemoodar{
    top: -3rem;
    right: 11.3rem;
}

.ft-btn:hover{
    &.ft-bg-light-red{
        background: linear-gradient(270deg, rgba(30, 62, 131, 1) 0%, rgba(18, 113, 169, 1) 50%, rgba(6, 159, 204, 1) 100%) !important;
    }
    &.ft-bg-light-blue{
        background: linear-gradient(90deg, rgba(183, 36, 109, 1) 0%, rgba(212, 65, 108, 1) 50%, rgba(247, 97, 107, 1) 100%);
    }
} 
</style>