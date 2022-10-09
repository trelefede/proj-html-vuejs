<template>
    <footer class="ft-bg-blue position-relative">
        
        <div class="container">
            <SubscribeComponent />
            <div class="row links">
                <div class="col-3">
                    <img src="@/assets/images/white-logo-2.png" alt="logo">
                    <p class="pe-3">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper impenetrable</p>
                </div>
                <div class="col-3" v-for="links in data" :key="links.id">
                    <FooterLinksComponent :links="links" />
                </div>
            </div>
            <SocialLinksComponent />
        </div>  
    </footer>
</template>

<script>
import SubscribeComponent from "@/components/SubscribeComponent.vue"
import FooterLinksComponent from "@/components/FooterLinksComponent.vue"
import SocialLinksComponent from "@/components/SocialLinksComponent.vue"

export default {
    name: "FooterComponent",
    props: {
        data: Array
    },
    components: {
        SubscribeComponent,
        FooterLinksComponent,
        SocialLinksComponent
    }
}
</script>

<style lang="scss" scoped>
footer{
    margin-top: 5rem;
    padding-top: 10rem;
    a, p{
        color: #786e7a;
        font-size: 0.9rem;
    }
}

.links{
    padding-bottom: 3rem;
}

 img{
    width: 45%;
    margin-bottom: 2rem;
 }
</style>