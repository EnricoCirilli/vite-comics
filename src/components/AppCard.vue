<script>
export default {
    props: {
        title: String,
        image: String,
    },
}


</script>

<template>

    <!-- card -->
    <div class="card">
        <img :src="image" alt="">
        <h3>{{ title }}</h3>
    </div>

</template>

<style lang="scss" scoped>

.card{
    height: 100%;
    
    img{
        height: 70%;
        width: 100%;
       object-fit: cover;
    }
}
h3{
    color: white;
}
</style>