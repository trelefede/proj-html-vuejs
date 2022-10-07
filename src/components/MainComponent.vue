<template>
    <main>
        <OurServicesComponent />
        <StartProjectComponent />
        <!-- <PortfolioComponent /> -->
        <PriceListComponent />
    </main>
</template>

<script>
import OurServicesComponent from "@/components/OurServicesComponent.vue"
import StartProjectComponent from "@/components/StartProjectComponent.vue"
import PriceListComponent from "@/components/PriceListComponent.vue"

export default {
    name: "MainComponent",
    components: {
        OurServicesComponent,
        StartProjectComponent,
        // PortfolioComponent,
        PriceListComponent

    }
}
</script>

<style lang="scss" scoped>

</style>