<template>
    <div class="start-project ft-bg-blue">
        <div class="container-lg">
            <div class="row align-items-center py-4 d-flex flex-row-reverse">
                <div class="col-6">
                    <p class="text-white">Start Your Project</p>
                    <h2 class="fw-bold">Grow Your Business</h2>
                    <h2 class="fw-light">With Our Strategy</h2>
                    <p class="py-4">When, while the lovely valley teems with vapour around <br> meand the meridian sun strikes the upper surface meand <br> the meridian sun strikes the upper surface</p>
                    <div class="d-flex justify-content-start pt-2">
                        <a class="btn rounded-pill ft-btn ft-bg-light-red me-4" href="#">Try It Now</a>
                        <a class="btn rounded-pill ft-btn ft-bg-light-blue" href="#">Explore More</a>
                    </div>
                </div>
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
</style>