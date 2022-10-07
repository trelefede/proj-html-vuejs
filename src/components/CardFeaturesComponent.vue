<template>
    <div :class="feature.id === 1 ? 'ft-text-white' : '' ">
        <p><span>Creative</span> {{ feature.creative }} </p>
        <p><span>Vibrant</span> {{ feature.vibrant }} </p>
        <p><span>Eye</span> {{ feature.eye }} </p>
        <p><span>Etreme</span> {{ feature.extreme }} </p>
        <p><span>Exceptional</span> {{ feature.exceptional }} </p>
    </div>
</template>

<script>
export default {
    name: "CardFeaturesComponent",
    props: {
        feature: Object
    },
}
</script>

<style lang="scss" scoped> 
.ft-text-white{
    
   
}

p{
    font-size: 0.9rem;
}

span{
    font-weight: bold;
    color: rgba(0, 0, 0, 0.708);
}
</style>