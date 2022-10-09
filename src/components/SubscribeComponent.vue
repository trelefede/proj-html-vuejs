<template>
    <div class="container  ft-bg-light-red subscribe">
        <div class="row align-items-center px-3">
            <div class="col-6">
                <h3 class="fw-bold text-white">We Offer Awesome Services</h3>
                <p class="text-white">When, while the lovely valley teems with vapour around meand meridian sun strikes upper surface .</p>
            </div>
            <div class="col-6 text-end d-flex justify-content-end">
                <div id="input-mail" class="d-flex justify-content-between">
                    <input class="fs-6 " type="text" placeholder="Enter Your Email Address">
                    <a class="btn rounded-pill ft-btn ft-bg-light-blue fs-6 ms-4" href="#">Subscribe</a>
                </div>
                 
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "SubscribeComponent",
}
</script>

<style lang="scss" scoped>
.subscribe{
    border-radius: 1.75rem;
    box-shadow: 1px -1px 70px 0px rgb(24 24 24 / 22%);
    padding: 4rem 2rem;
    position: absolute;
    top: -25%;
    transform: translateY(8%);
};

p{
    font-size: 0.81rem;
    margin: 0;
}

h3{
    font-size: 2.2rem;
}

.ft-btn{
    padding-right: 1.3rem;
    padding-left: 1.3rem;
}

#input-mail{
    background-color: white;
    width: 75%;
    border-radius: 50rem;
    padding: 5px 7px;
    input{
        border-style: none;
        margin-left: 1rem;
        flex-grow: 1;
    }
    ::placeholder{
        color: #c5c5c5;
    }
}


</style>