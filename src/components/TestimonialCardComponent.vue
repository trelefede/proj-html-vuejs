<template>
    <div class="card text-center">
        <div class="card-body mx-4 position-relative">

            <!-- card image -->
            <img :src="require (`@/assets/images/${card.img}`)" :alt="card.author">

            <!-- rating element with stars -->
            <div class="rating mb-4 position">
                <p class="markers">//</p>
                <font-awesome-icon class="full-star" icon="fa-solid fa-star" v-for="stars in card.fullStars" :key="stars" />
                <font-awesome-icon icon="fa-regular fa-star" v-for="stars in card.emptyStars" :key="stars" />
            </div>

            <!-- card content -->
            <p class="my-4"> {{ card.review }} </p>
            <p class="fw-bold text-dark mb-1"> {{ card.author }} </p>
            <p> {{ card.position }} </p>
        </div>
    </div>
</template>

<script>
export default {
    name: "TestimonialCardComponent",
    props: {
        card: Object
    },
}
</script>

<style lang="scss" scoped>
.card{
    border: none;
    margin-top: 5rem;
    z-index: 9999;
}

img{
    width: 27%;
    border: 4px solid #b6256f;
    border-radius: 50%;
    margin-bottom: 3rem;
}

.full-star{
        color: rgb(183, 36, 109);
        color: linear-gradient(90deg, rgba(183, 36, 109, 1) 0%, rgba(212, 65, 108, 1) 50%, rgba(247, 97, 107, 1) 100%);    
}

p{
    color: #4e4e4e;
    font-size: 0.8rem;
}

.markers{
    position: absolute;
    font-size: 3.8rem;
    font-weight: 900;
    color: #eee;
    z-index: -1;
    top: 8.1rem;
    right: 45%;
}
</style>