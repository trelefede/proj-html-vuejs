<template>
    <div class="container">
        <div class="row align-items-center">

            <!-- create elements with v-for -->
            <div class="col cliently" v-for="customer in clientlyData" :key="customer">
                <img :src="require (`@/assets/images/${customer}`)" :alt="customer">
            </div>
        </div>
    </div>
</template>

<script>
import { clientlyData } from "@/data/data.js"

export default {
    name: "ClientlyComponent",
    data(){
        return {
            clientlyData
        }
    },
}
</script>

<style lang="scss" scoped>
.container{
    height: 300px;
}

.cliently{
    margin-top: 8rem;
    margin-bottom: 7rem;
    text-align: center;
    img{
        width: 45%;
    }
}
</style>