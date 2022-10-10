<template>
    <header class="ft-bg-blue">
        <div class="container">

            <!-- navbar with logo, site links and user sign in -->
            <div class="navbar d-flex justify-between py-3">
                <div class="logo">
                    <img src="@/assets/images/white-logo-2.png" alt="logo">
                </div>
                <div class="links d-flex justify-between align-items-center">
                    <div class="me-4">
                        <ul class="list-inline mt-3">
                            <li class="list-inline-item px-2" v-for="link in data" :key="link"> 
                                <a href="#" :class="link === 'Home' ? 'active' : 'text-white'" > {{ link }} </a> 
                            </li>
                        </ul>
                    </div>
                    <div class="ms-4">
                        <a class="btn rounded-pill ft-btn ft-bg-light-blue" href="#" role="button">Sign In</a>
                    </div>
                </div>
            </div>
            <!-- end navbar -->

            <!-- jumbotron -->
            <JumbotronComponent />
        </div>
    </header>
</template>

<script>
import JumbotronComponent from "@/components/JumbotronComponent.vue"

// creare componente jumbotron

export default {
    name: "HeaderComponent",
    props: {
        data: Array,
    },
    components: {
        JumbotronComponent,
    },
}
</script>

<style lang="scss" scoped>
.ft-btn{
    padding-right: 1.3rem;
    padding-left: 1.3rem;
}

li{
    a{
        &.active{
            color: #f6636a;
        }
    }
}
</style>