<template>
    <div id="portfolio">
        <div class="container">
            <div class="row mb-4">

                <!-- heading text -->
                <div class="col-6">
                    <p class="mt-4 mb-2 ft-color-red">Portfolio</p>
                    <h3 class="fw-light fs-1 mb-3"><span class="fw-bold">latest</span> work</h3>
                </div>

                <!-- carousel controls -->
                <div class="col-6 ft-arrows d-flex justify-content-end align-items-end">
                    <button>
                        <font-awesome-icon icon="fa-solid fa-arrow-left" />
                    </button>
                    <button>
                        <font-awesome-icon icon="fa-solid fa-arrow-right" class="ms-2" />
                    </button>
                </div>
            </div>
        </div>

        <!-- CAROUSEL SECTION -->
        <CarouselComponent />

        <!-- carousel image displays -->
        <div class="row mt-4">
            <div class="col-12 ft-dot d-flex justify-content-center">
               <font-awesome-icon icon="fa-solid fa-circle" class="active" />
               <font-awesome-icon icon="fa-solid fa-circle" />
               <font-awesome-icon icon="fa-solid fa-circle" />
               <font-awesome-icon icon="fa-solid fa-circle" />
               <font-awesome-icon icon="fa-solid fa-circle" />
            </div>
        </div>
    </div>
</template>

<script>
import CarouselComponent from "@/components/CarouselComponent.vue"

export default {
    name: "PortfolioComponent",
    components: {
        CarouselComponent
    },
}
</script>

<style lang="scss" scoped>
#portfolio{
    margin-bottom: 4rem;
    margin-top: 4rem;
}

button{
    background: none;
    border: none;
}

.ft-arrows{
    svg{
        border-radius: 50%;
        border: 1px #fa8a90 solid;
        color: #fa8a90;
        padding: 11px 12px;
    }
}

.ft-dot{
    margin-top: 4rem;
    svg{
        color: #e5e5e9;
        margin: 0.2rem;
        font-size: 0.5rem;
        &.active{
            color: #fa8a90;
        }
    }
}
</style>