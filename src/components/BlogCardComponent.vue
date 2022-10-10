<template>
    <div>
        <!-- card -->
        <div class="card ft-card" :class="card.id  === 0 ? 'card-large' : 'ft-bg-blue'">
            <div class="card-body py-4 my-3" :class="card.id  === 0 ? 'card-large-body' : ''">
                
                <!-- card header -->
                <div>
                    <div class="heading d-flex">
                        <p> {{ card.date }} </p>
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-dot" viewBox="0 0 16 16">
                            <path d="M8 9.5a1.5 1.5 0 1 0 0-3 1.5 1.5 0 0 0 0 3z"/>
                        </svg>
                        <p>by {{ card.author }} </p>
                    </div>

                    <!-- card main -->
                    <h5 class="my-3"> {{ card.title }} </h5>
                    <p> {{ card.content }} </p>  
                </div>

                    <!-- card button -->
                <div>
                    <a class="btn rounded-pill ft-btn mt-2" href="#">Read More</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "BlogCardComponent",
    props: {
        card: Object
    },
}
</script>

<style lang="scss" scoped>
.card-large{
    background-image: url(@/assets/images/headway-537308-unsplash-1380x703.jpg);
    background-size: cover;
    background-position-x: right;
    box-shadow: inset 0px 0px 20px 1000px rgb(18 15 15 / 50%) !important;
    height: 100%;
}

.card-large-body{
    flex-direction: row !important;
    align-items: flex-end !important;
    color: white;
    > div{
        max-width: 70%;
    }
    div :last-child{
        margin-bottom: 19px;
    }
}

.card{
    height: 100%;
}

.card-body{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: space-around;
    margin-left: 1rem;
    margin-right: 1rem;
    font-size: 0.8rem;
}

.ft-bg-blue{
    background: linear-gradient(167deg, #01000a 0%, #030a55 100%, #000 100%);
}
.ft-card{
    border-radius: 1.75rem;
    box-shadow: 1px -1px 70px 0px rgb(24 24 24 / 22%);
    margin-top: 5rem;
}
.ft-btn{
    color:#252525cc;
    background-color: white;
    font-size: 0.8rem;
}

h5{
    font-size: 1.15rem;
}

p{
    color: #cdcdcd;
}
</style>