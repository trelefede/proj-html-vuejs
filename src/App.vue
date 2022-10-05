<template>
  <div id="app">
    <HeaderComponent :data="headerData" />
    <MainComponent />
    <FooterComponent :data="footerData" />
  </div>
</template>

<script>
import HeaderComponent from "@/components/HeaderComponent.vue"
import MainComponent from "@/components/MainComponent.vue"
import FooterComponent from "@/components/FooterComponent.vue"

import { headerData } from "@/data/data.js"
import { footerData } from "@/data/data.js"

export default {
  name: 'App',
  data(){
    return {
      headerData,
      footerData
    }
  },
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent
  }
}
</script>

<style lang="scss">
@import '~bootstrap';

</style>
