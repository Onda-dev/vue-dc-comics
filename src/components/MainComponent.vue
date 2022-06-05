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
                        <li>
                            <a href="#">digital comics</a>
                        </li>
                        <li>
                            <a href="#">dc merchandise</a>
                        </li>
                        <li>
                            <a href="#">subscription</a>
                        </li>
                        <li>
                            <a href="#">comic shop locator</a>
                        </li>
                        <li>
                            <a href="#">dc power visa</a>
                        </li>
                    </ul>  
                </nav>
            </div> 
        </div>

    </main>
</template>

<script>
export default {
    name: 'MainComponent'
}
</script>

<style>
.content {
    background-color: black;
    padding: 3.75rem;
    display: flex;
    justify-content: center;
}
.main-nav-box {
    background-color: var(--first-color);
    padding: 3.75rem;
}
main ul {
    display: flex;
    gap: 6.25rem;
}
main ul li {
    display: inline-block;

}

</style>