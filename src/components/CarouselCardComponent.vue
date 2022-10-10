<template>
    <div class="card" style="width: 18rem;">
        <img :src="require(`@/assets/images/${card.img}`)" class="card-img-top" :alt="card.title">
        <div class="card-body">
            <h5 class="card-title"> {{ card.title }} </h5>
            <p class="card-text"> {{ card.subtitle }} </p>
        </div>
    </div>
</template>

<script>
export default {
    name: "CarouselCardComponent",
    props: {
        card: Object
    }
}
</script>

<style lang="scss" scoped>

</style>