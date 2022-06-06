<template>
    <main>
        <div class="content">
            <div class="container">
                <SectionProducts/>
            </div>
        </div>
        <div class="main-nav-box">
            <div class="main-nav container">
                <nav>
                    <ul>
                        <li v-for="(link, index) in links" :key="index">
                            <img :src="link.img" alt="">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>  
                </nav>
            </div> 
        </div>
    </main>
</template>

<script>
import SectionProducts from '../components/sections/SectionProducts.vue'

export default {
    name: 'MainComponent',
    components: {
        SectionProducts
    },
    data() {
        return {
            links: [
                {
                    text: "digital comics",
                    url: "#",
                    img: "/img/buy-comics-digital-comics.png"
                },
                {
                    text: "dc merchandise",
                    url: "#",
                    img: "/img/buy-comics-merchandise.png"
                },
                {
                    text: "subscription",
                    url: "#",
                    img: "/img/buy-comics-shop-locator.png"
                },
                {
                    text: "comic shop locator",
                    url: "#",
                    img: "/img/buy-comics-subscriptions.png"
                },
                {
                    text: "dc power visa",
                    url: "#",
                    img: "/img/buy-dc-power-visa.svg"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.container {
    max-width: var(--main-container);
}
.content {
    background-color: #1C1C1C;
    padding: 3.75rem;
}
.main-nav-box {
    background-color: var(--first-color);
    padding: 3.75rem;
}
main ul {
    display: flex;
    justify-content: center;
    gap: 2.5rem;
}
main ul li {
    display: flex;
    align-items: center;
    gap: .625rem;

}
img {
    max-width: 3.125rem;
    max-height: 3.125rem;
}
</style>