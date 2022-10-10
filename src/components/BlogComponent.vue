<template>
    <div class="container blog">
        
        <!-- heading section  -->
        <div class="row">
            <div class="col-12 text-center">
                <p class="mt-4 mb-2 ft-color-red">Blog</p>
                <h3 class="fw-light fs-1 mb-3"><span class="fw-bold">Latest</span> Posts</h3>
                <p id="heading-content">When, while the lovely valley teems with vapour around meand the meridian sun strikes <br> the upper surface .</p>
            </div>
        </div>

        <!-- content section create by data.js-->
        <div class="row">
            <BlogCardComponent :class="cardData.id === 0 ? 'col-6' : 'col-3'" 
            v-for="cardData in blogData" :key="cardData.id" 
            :card="cardData" />
        </div>
    </div>
</template>

<script>
import BlogCardComponent from "@/components/BlogCardComponent.vue"

import { blogData } from "@/data/data.js"

export default {
    name: "BlogComponent",
    data(){
        return {
            blogData
        }
    },
    components: {
        BlogCardComponent,
    },
}
</script>

<style lang="scss" scoped>
.blog{
    margin-top: 25rem;
    margin-bottom: 10rem;
}

#heading-content{
    color:#252525cc
}
</style>