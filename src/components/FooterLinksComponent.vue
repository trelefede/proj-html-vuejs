<template>
    <div>
        <h6> {{ links.title }} </h6>
        <a href="#" class="d-flex direction-column" v-for="link in links.info" :key="link" > {{ link }} </a>
        <div :class="links.id === 2 ? '' : 'd-none'">
            <p class="mt-4 pt-2"><span>Address:</span> {{ links.address }} </p>
            <p><span>Phone:</span> {{ links.phone }} </p>
            <p><span>Email:</span> {{ links.email }} </p>
        </div>
    </div>
</template>

<script>

export default {
    name: "FooterLinksComponent",
    props: {
        links: Object
    }
}
</script>

<style lang="scss" scoped>
a{
    font-style: none;
    font-size: 0.8rem;
    color: #71728d;
    line-height: 2rem;
}

p{
    color: #71728d;
    font-size: 0.8rem;
}

span{
    font-weight: bold;
    color: white;
}
</style>