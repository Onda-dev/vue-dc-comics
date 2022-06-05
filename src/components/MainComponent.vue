<template>
    <main>
        <div class="content">
            <div class="container">
                <div class="content-box">
                    <h1>Content goes here</h1>
                </div>
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
export default {
    name: 'MainComponent',
    data() {
        return {
            links: [
                {
                    text: "digital comics",
                    url: "#",
                    img: "./assets/img/buy-comics-digital-comics.png"
                },
                {
                    text: "dc merchandise",
                    url: "#",
                    img: "../assets/img/buy-comics-merchandising.png"
                },
                {
                    text: "subscription",
                    url: "#",
                    img: "../assets/img/subscriptions.png"
                },
                {
                    text: "comic shop locator",
                    url: "#",
                    img: "../assets/img/buy-comics-shop-locator.png"
                },
                {
                    text: "dc power visa",
                    url: "#",
                    img: "../assets/img/power-visa.png"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.content {
    background-color: black;
    padding: 3.75rem;
}
.main-nav-box {
    background-color: var(--first-color);
    padding: 3.75rem;
}
main ul {
    display: flex;
    justify-content: center;
    gap: 6.25rem;
}
main ul li {
    display: inline-block;

}
</style>