<template>
    <div>
        <!-- heading section  -->
        <div class="row">
            <div class="col-12 text-center">
                <p class="mt-4 mb-2 ft-color-red">Blog</p>
                <h3 class="fw-light fs-1 mb-3"><span class="fw-bold">Latest</span> Posts</h3>
                <p>When, while the lovely valley teems with vapour around meand the meridian sun strikes <br> the upper surface .</p>
            </div>
        </div>

        <!-- content section create by data.js-->
        <div class="row">
            <BlogCardComponent />
        </div>
    </div>
</template>

<script>
export default {
    name: "BlogComponent",
}
</script>

<style lang="scss" scoped>

</style>