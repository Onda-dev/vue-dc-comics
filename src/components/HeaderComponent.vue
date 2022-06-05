<template>
    <header class="header container">
        <div class="header__logo">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
        </div>
        <nav class="header__nav">
            <ul>
                <li v-for="(link, index) in links" :key="index" :class="{active : link.current}">
                    <a :href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'HeaderComponent',
    data() {
        return {
            links: [
                {
                    text: "characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "games",
                    url: "#",
                    current: false,
                },
                {
                    text: "collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "news",
                    url: "#",
                    current: false,
                },
                {
                    text: "shop",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.25rem 0;
    
    &__nav {
        ul {
            display: flex;
            flex-direction: row;
        }
    }

    &__nav {
        ul {
            li {
                padding: 1.25rem;
            }
        }
    }
}

</style>