<template>
    <main>
        <OurServicesComponent />
        <StartProjectComponent />
        <!-- <PortfolioComponent /> -->
        <PriceListComponent />
        <BlogComponent />
        <TestimonialComponent />
        <ClientlyComponent />
    </main>
</template>

<script>
import OurServicesComponent from "@/components/OurServicesComponent.vue"
import StartProjectComponent from "@/components/StartProjectComponent.vue"
import PriceListComponent from "@/components/PriceListComponent.vue"
import BlogComponent from "@/components/BlogComponent.vue"
import TestimonialComponent from "@/components/TestimonialComponent.vue"
import ClientlyComponent from "@/components/ClientlyComponent.vue"

export default {
    name: "MainComponent",
    components: {
        OurServicesComponent,
        StartProjectComponent,
        // PortfolioComponent,
        PriceListComponent,
        BlogComponent,
        TestimonialComponent,
        ClientlyComponent,
    }
}
</script>

<style lang="scss" scoped>

</style>