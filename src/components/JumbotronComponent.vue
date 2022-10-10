<template>
    <div class="jumbotron">
        <div class="row align-items-center py-4">

            <!-- left panel -->
            <div class="col-6 mt-4 pt-4">
                <h2 class="fw-bold">Business Planning</h2>
                <h2 class="fw-light">Digital Technology</h2>
                <h2 class="fw-bold">Modern Solution !</h2>
                <p class="py-4">When, while the lovely valley teems with vapour around <br> meand the meridian sun strikes the upper surface .</p>

                <!-- user buttons -->
                <div class="d-flex justify-content-start pt-2">
                    <a id="btn-try-now" class="btn rounded-pill ft-btn ft-bg-light-red me-4" href="#">Try It Now</a>
                    <a id="btn-explore-more" class="btn rounded-pill ft-btn ft-bg-light-blue" href="#">Explore More</a>
                </div>
            </div>

            <!-- right panel -->
            <div class="col-6 d-flex justify-content-end">
                <img src="@/assets/images/header.png" alt="jumbotron planning">
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name: "JumbotronComponent"
}
</script>

<style lang="scss" scoped>
.jumbotron{
    padding-bottom: 10rem;
}
h2{
    font-size: 3.3rem;
}

p{
    color: #017999e6;
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