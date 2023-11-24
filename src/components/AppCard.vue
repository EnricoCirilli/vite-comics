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
    img{
        width: 100%;
    }
}

</style>