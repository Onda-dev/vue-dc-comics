<template>
    <div class="footer">
        <div class="footer-top">
            <div class="container">
                <nav>
                    <ul>
                        <h3>dc comics</h3>
                        <li v-for="(link, index) in DcComicsLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                    <ul>
                        <h3>shop</h3>
                            <li v-for="(link, index) in ShopLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                    <ul>
                        <h3>dc</h3>
                            <li v-for="(link, index) in DcLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                    <ul>
                        <h3>sites</h3>
                            <li v-for="(link, index) in SitesLinks" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                        </li>
                    </ul>
                </nav>
                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
                </div>
            </div>
        </div>

        <div class="footer-bottom">
            <div class="container">
                <button type="button">
                sign up now
                </button>
                <nav>
                    <ul>
                        <h3>follow us</h3>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-facebook.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-twitter.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-youtube.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-pinterest.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-periscope.png" alt="">
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterComponent',
    data() {
        return {
            DcComicsLinks: [
                {
                    text: "Characters",
                    url: "#",
                },
                {
                    text: "Comics",
                    url: "#",
                },
                {
                    text: "Movies",
                    url: "#",
                },
                {
                    text: "TV",
                    url: "#",
                },
                {
                    text: "Games",
                    url: "#",
                },
                {
                    text: "Videos",
                    url: "#",
                },
                {
                    text: "News",
                    url: "#",
                },
            ],
            ShopLinks: [
                {
                    text: "Shop DC",
                    url: "#",
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#",
                },
            ],
            DcLinks: [
                {
                    text: "Terms Of Use",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                },
                {
                    text: "Privacy Policy(New)",
                    url: "#",
                }
            ],
            SitesLinks: [
                {
                    text: "DC",
                    url: "#",
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
.footer-top {
    padding: 3.75rem 0;
    background-image: url(../assets/img/footer-bg.jpg);
    height: 500px;
    overflow: hidden;

    .container {
        display: flex;
        justify-content: space-between;
    }

    img {
        margin-top: -100px;
    }
}

.footer nav {
    display: flex;
    gap: 2.5rem;
}

.footer li {
    padding: .5rem 0;
}

.footer-bottom {
    background-color: var(--second-color);
    padding: 3.75rem;
    
    .container {
        display: flex;
        justify-content: space-between;

        button {
            padding: 1.25rem;
            height: 100%;
            background-color: rgba($color: #000000, $alpha: 0);
            border: .125rem solid var(--first-color);
        }
    }
}
</style>