<template>
    <main>
        <OurServicesComponent />
        <StartProjectComponent />
        <!-- <PortfolioComponent /> -->
        <PriceListComponent />
        <BlogComponent />
    </main>
</template>

<script>
import OurServicesComponent from "@/components/OurServicesComponent.vue"
import StartProjectComponent from "@/components/StartProjectComponent.vue"
import PriceListComponent from "@/components/PriceListComponent.vue"
import BlogComponent from "@/components/BlogComponent.vue"

export default {
    name: "MainComponent",
    components: {
        OurServicesComponent,
        StartProjectComponent,
        // PortfolioComponent,
        PriceListComponent,
        BlogComponent
    }
}
</script>

<style lang="scss" scoped>

</style>