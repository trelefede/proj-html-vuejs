<template>
    <div class="card" style="width: 18rem;">
        <img :src="require(`@/assets/images/${card.img}`)" class="card-img-top" :alt="card.title">
        <div class="card-body d-flex justify-content-between align-items-center">
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
.card{
    width: 23rem !important;
    border-radius: 1rem;
    border: none;
    margin-left: 1rem;
    margin-right: 1rem;
    box-shadow: 1px -1px 70px 0px rgb(24 24 24 / 22%);
    img{
        border-radius: 1rem;
    }
    .card-title{
        text-align: start;
        font-size: 0.9rem;
        font-weight: bold;
        margin-bottom: 0;
    }
    .card-text{
        text-align: end;
        font-size: 0.9rem;
    }
}
</style>