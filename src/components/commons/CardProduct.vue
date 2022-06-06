<template>
    <div class="product">
        <img :src="image" :alt="title">
        <h3>{{title}}</h3>
    </div>
</template>

<script>
export default {
    name: 'CardProduct',
    props: {
        title: String,
        image: String
    }
}
</script>

<style lang="scss" scoped>

</style>