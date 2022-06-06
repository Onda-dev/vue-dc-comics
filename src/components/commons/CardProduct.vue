<template>
    <div class="product">
        <div class="img-box">
            <img :src="image" :alt="title">
        </div>
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
.product {
    width: 9.375rem;
    display: flex;
    flex-direction: column;
    gap: .875rem;

    img {
        width: 9.375rem;
    }
}

.img-box {
    height: 9.375rem;
    width: 9.375rem;
    overflow: hidden;
}

    
</style>