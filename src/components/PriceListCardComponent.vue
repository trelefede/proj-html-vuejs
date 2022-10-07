<template>
    <div>
        <div class="card ft-card position-relative text-center" :class="cards.title === 'Developing' ? 'ft-bg-light-red' : ''" >
            <div class="card-body mx-4">
                <h5 class="text-dark fs-2 fw-bold"> {{ cards.title }} </h5>
                <h6 class="text-dark mb-4 mt-3"> {{ cards.subtitle.toUpperCase() }} </h6>
                <span class="text-dark ft-price-type d-block mt-2">$</span>
                <h6 class="ft-price text-dark fw-bold mb-2"> {{ cards.price }} </h6>
                <span class="ft-price-bg" :class="cards.title === 'Developing' ? 'ft-bg-red' : ''" > {{ cards.price }} </span>
                <span class="text-dark"> {{ cards.billing }} </span>
                <CardFeaturesComponent :feature="cards.features" />
            </div>
        </div>
    </div>
</template>
<!--    -->
<script>
import CardFeaturesComponent from "@/components/CardFeaturesComponent.vue"

export default {
    name: "PriceListCardComponent",
    props: {
        cards: Object
    },
    components: {
        CardFeaturesComponent
    }
}
</script>

<style lang="scss" scoped>
.ft-card{
    z-index: 9999;
    margin-top: 5rem;
    border-radius: 1.75rem;
}

.ft-price{
    font-size: 5rem;
}

.ft-price-bg{
    color: #e9e9e9;
    font-size: 15rem;
    position: absolute;
    z-index: -1;
    top: -6.2rem;
    right: -0.7rem;
}

.ft-bg-red{
    color: #e9e9e93d !important;
}

h6{
    font-size: 0.8rem;
}
</style>