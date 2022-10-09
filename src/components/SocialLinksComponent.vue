<template>
    <div id="footer" class="row align-items-center">
        <div class="col-6 d-flex align-items-baseline">
            <font-awesome-icon icon="fa-regular fa-copyright" />
            <p>2020 Phlox. All Right Reserved.</p>
        </div>
        <div id="brands" class="col-6 d-flex justify-content-end">
            <div class="d-flex text-white align-self-center">
                <font-awesome-icon icon="fa-brands fa-instagram" />
                <font-awesome-icon icon="fa-brands fa-linkedin-in" />
                <font-awesome-icon icon="fa-brands fa-facebook-f" />
                <font-awesome-icon icon="fa-brands fa-twitter" />
            </div>
            <div id="arrow-up"><font-awesome-icon icon="fa-solid fa-arrow-up" /></div>
            <div id="chat" class="align-self-center"><font-awesome-icon icon="fa-regular fa-comment" /></div>
        </div>
    </div>
</template>

<script>
export default {
    name: "SocialLinksComponent"
}
</script>

<style lang="scss" scoped>
#footer{
    height: 80px;
    border-top: 1px solid #ffffff1a;
}

svg{
    font-size: 1rem;
    margin: 1rem;
}

p{
    font-size: 0.8rem
}

#brands{
    height: 100%;
}

#arrow-up{
    background-color: #ffffff;
    border-radius: 50%;
    align-self: flex-start;
    margin: 0 1rem;
    svg{
        color: black;
        margin: 0;
        transform: translateY(1px);
        padding: 2px 7px;
        font-size: 0.8rem;
    }
}

#chat{
    font-size: 1.5rem;
    background-color: #517cea;
    border-radius: 50%;
    svg{
        margin: 0;
        font-size: 1.8rem;
        padding: 9px 13px;
        transform: translateY(2px);
        transform: translateX(1px);
    }
}
</style>