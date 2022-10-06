<template>
    <div class="jumbotron">
        <div class="row align-items-center py-4">
            <div class="col-6">
                <h2 class="fw-bold">Business Planning</h2>
                <h2 class="fw-light">Digital Technology</h2>
                <h2 class="fw-bold">Modern Solution !</h2>
                <p class="py-4">When, while the lovely valley teems with vapour around <br> meand the meridian sun strikes the upper surface .</p>
                <div class="d-flex justify-content-start pt-2">
                    <a class="btn rounded-pill ft-btn-light-red me-4" href="#">Try It Now</a>
                    <a class="btn rounded-pill ft-btn-light-blue" href="#">Explore More</a>
                </div>
            </div>
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
    color: #fff;
    font-size: 3.3rem;
}

p{
    color: #017999e6;
}
</style>