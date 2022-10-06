<template>
    <div class="container-lg">
        <!-- heading section  -->
        <div class="row">
            <div class="col-12 text-center">
                <p class="mt-4 mb-2 ft-color-red">Our Services</p>
                <h3 class="fw-light fs-1"><span class="fw-bold">What</span> We Do</h3>
                <p>When, while the lovely valley teems with vapour around meand</p>
            </div>
        </div>

            <!-- content section -->
        <div class="row ft-content">
            <div class="col-3 text-center">
                <img src="@/assets/images/Group-247.png" alt="data analisys">
                <h4 class="fw-bold pb-3">Data Analysis</h4>
                <p class="fs-6 px-4">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper</p>
            </div>
            <div class="col-3 text-center">
                <img src="@/assets/images/Group-567.png" alt="data analisys">
                <h4 class="fw-bold pb-3">SEO Optimization</h4>
                <p class="fs-6 px-4">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper</p>
            </div>
            <div class="col-3 text-center">
                <img src="@/assets/images/Group-538.png" alt="data analisys">
                <h4 class="fw-bold pb-3">Security Data</h4>
                <p class="fs-6 px-4">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper</p>
            </div>
            <div class="col-3 text-center">
                <img src="@/assets/images/Group-566.png" alt="data analisys">
                <h4 class="fw-bold pb-3">Branding Strategy</h4>
                <p class="fs-6 px-4">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper</p>
            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center mb-4 pb-4">
                <a class="btn rounded-pill ft-btn ft-bg-light-red mb-4" href="#">View All Services</a>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "OurServicesComponent",
    components: {
    }
}
</script>

<style lang="scss" scoped>
img{
    width: 50%;
    height: 7.5rem;
    margin-bottom: 4rem;
}

p{
    font-size: 0.9rem;
}

.ft-content{
    margin-top: 8rem;
    margin-bottom: 10rem;
}

a{
    box-shadow: 1px -1px 70px 0px rgba(232,43,43,0.66);;
}
</style>