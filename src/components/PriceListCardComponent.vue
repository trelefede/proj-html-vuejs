<template>
    <div>
        <div class="card ft-card position-relative text-center" :class="cards.title === 'Developing' ? 'ft-bg-light-red' : 'color-black'" >
            <div class="card-body mx-4">
                <h5 class="fs-2 fw-bold mt-4"> {{ cards.title }} </h5>
                <h6 class="mb-4 mt-3"> {{ cards.subtitle.toUpperCase() }} </h6>
                <span class="ft-price-type d-block mt-2">$</span>
                <h6 class="ft-price fw-bold mb-2"> {{ cards.price }} </h6>
                <span class="ft-price-bg" :class="cards.title === 'Developing' ? 'ft-bg-red' : ''" > {{ cards.price }} </span>
                <span> {{ cards.billing }} </span>
                <CardFeaturesComponent :feature="cards.features" class="my-4"/>
                <a class="btn rounded-pill ft-btn my-4" :class="cards.title === 'Developing' ?'ft-bg-white' : 'ft-bg-light-red'" href="#">
                    Order Now 
                    <font-awesome-icon icon="fa-solid fa-arrow-right" />
                </a>
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
    margin-top: 6rem;
    margin-bottom: 7rem;
    border-radius: 1.75rem;
    box-shadow: 1px -1px 70px 0px rgb(24 24 24 / 22%);
}

.ft-price{
    font-size: 5rem;
}

.ft-price-type{
    padding-right: 7rem;
}

.ft-price-bg{
    color: #e9e9e9;
    font-size: 15rem;
    position: absolute;
    z-index: -1;
    top: -6.2rem;
    right: -0.7rem;
}

.color-black{
    color: black;
}

.ft-bg-light-red{
    background: linear-gradient(131deg, #b7246d 0%, #d4416c 50%, #f7616b 100%);
}
.ft-bg-red{
    color: #e9e9e93d !important;
}

.ft-bg-white{
    background-color: white;
    color:  #d4416c;
    font-weight: 500;
}

h6{
    font-size: 0.8rem;
}

a{
    box-shadow: 1px -1px 70px 0px rgba(232, 43, 43, 0.483);
    svg{
        margin-left: 3rem;
    }
    &.ft-bg-light-red{
        background: linear-gradient(179deg, #b7246d 0%, #d4416c 50%, #f7616b 100%);
    }
}
</style>