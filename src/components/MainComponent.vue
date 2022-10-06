<template>
    <main>
        <OurServicesComponent />
        <StartProjectComponent />
    </main>
</template>

<script>
import OurServicesComponent from "@/components/OurServicesComponent.vue"
import StartProjectComponent from "@/components/StartProjectComponent.vue"

export default {
    name: "MainComponent",
    components: {
        OurServicesComponent,
        StartProjectComponent

    }
}
</script>

<style lang="scss" scoped>

</style>