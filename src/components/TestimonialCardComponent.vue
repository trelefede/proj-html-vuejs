<template>
    <div class="card">
        <div class="card-body">
            <img :src="`${imgUrl}${card.img}`" :alt="card.author">
            
        </div>
    </div>
</template>

<script>
export default {
    name: "TestimonialCardComponent",
    data(){
        return{
            imgUrl: '@/assets/images/'
        }
    },
    props: {
        card: Object
    },
}
</script>

<style lang="scss" scoped>

</style>