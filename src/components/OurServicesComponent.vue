<template>
    <div class="container">
        
        <!-- heading section  -->
        <div class="row mt-4 pt-2">
            <div class="col-12 text-center">
                <p class="mt-4 mb-2 ft-color-red">Our Services</p>
                <h3 class="fw-light fs-1"><span class="fw-bold">What</span> We Do</h3>
                <p>When, while the lovely valley teems with vapour around meand</p>
            </div>
        </div>

        <!-- content section create by data.js-->
        <div class="row ft-content">
            <div class="col-3 text-center ft-card" v-for="data in ourServicesData" :key="data.title">
                <div class="ft-card-img">
                    <img :src="require (`@/assets${data.img}`)" :alt="data.title">
                </div>
                <h4 class="fw-bold pb-3"> {{ data.title }} </h4>
                <p class="fs-6 px-4"> {{ data.info }} </p>
                <font-awesome-icon icon="fa-solid fa-arrow-right" />
            </div>
        </div>

        <!-- button -->
        <div class="row">
            <div class="col-12 text-center mb-4 pb-4">
                <a class="btn rounded-pill ft-btn ft-bg-light-red mb-4" href="#">View All Services</a>
            </div>
        </div>
    </div>
</template>

<script>
import { ourServicesData } from "@/data/data.js"


export default {
    name: "OurServicesComponent",
    data(){
        return {
            ourServicesData
        }
    },
}
</script>

<style lang="scss" scoped>
img{
    width: 50%;
    height: 7.5rem;
    margin-bottom: 4rem;
}

p{
    font-size: 0.9rem;
}

.ft-content{
    margin-top: 8rem;
    margin-bottom: 10rem;
}

svg{
    display: none;
}

.ft-card:hover{
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    color: white;
    background: linear-gradient(0deg, #090434 0%, #0815a3 100%, #000 100%);
    box-shadow: 1px -1px 70px 0px rgb(24 24 24 / 22%);
    border-radius: 2rem;
    .ft-card-img{
        position: absolute;
        background-color: white;
        box-shadow: 1px -1px 70px 0px rgb(24 24 24 / 22%);
        padding: 2rem;
        border-radius: 2rem;
        top: -30%;
        left: 17%;
    }
    img{
        margin: 0;
        width: 100%;
    }
    p{
        margin-bottom: 3rem;
        color: #fff;
        line-height: 2rem;
    }
    svg{
        display: inline-block;
        position: absolute;
        color: white;
        background: linear-gradient(90deg, rgba(183, 36, 109, 1) 0%, rgba(212, 65, 108, 1) 50%, rgba(247, 97, 107, 1) 100%);
        border-radius: 50%;
        bottom: -2rem;
        padding: 1.2rem 1.3rem;
        left: 50%;
        font-size: 1.8rem;
        transform: translatex(-50%);
    }
}

a{
    box-shadow: 1px -1px 70px 0px rgba(232, 43, 43, 0.483);
}
</style>