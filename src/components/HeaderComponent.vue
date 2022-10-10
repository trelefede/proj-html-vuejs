<template>
    <header class="ft-bg-blue">
        <div class="container">

            <!-- NAVBAR -->
            <div class="navbar d-flex justify-between py-3">

                <!-- logo -->
                <div class="logo">
                    <img src="@/assets/images/white-logo-2.png" alt="logo">
                </div>

                <!-- links -->
                <div class="links d-flex justify-between align-items-center">
                    <div class="me-4">
                        <ul class="list-inline mt-3">

                            <!-- links list -->
                            <li class="list-inline-item px-2" v-for="link in data" :key="link"> 
                                <a href="#" :class="link === 'Home' ? 'active' : 'text-white'" > {{ link }} </a> 
                            </li>
                        </ul>
                    </div>

                    <!-- button user sign in -->
                    <div class="ms-4">
                        <a class="btn rounded-pill ft-btn ft-bg-light-blue" href="#" role="button">Sign In</a>
                    </div>
                </div>
            </div>

            <!-- JUMBOTRON -->
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