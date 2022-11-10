<script>
export default {
    name: 'SiteMain',
    data() {
        return {
            icons: [
                {
                    image: '../assets/img/buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    image: '../assets/img/buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    image: '../assets/img/buy-comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    image: '../assets/img/buy-comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    image: '../assets/img/buy-dc-power-visa.svg',
                    text: 'dc power visa'
                },
            ]
        }
    }
}
</script>
<template>
    <main id="site_main">
        <section class="goes_here">
            <div class="container">
                <h2 class="text-white">--> Content goes here >-- </h2>
            </div>
        </section>
        <section class="icons">
            <div class="container">
                <div class="row">
                    <div class="col d-flex align-items-center" v-for="icon in icons">
                        <div class="logo">
                            <img :src="icon.image" alt="">
                        </div>
                        <div class="description ps-3">
                            <h6 class="text-uppercase text-white">{{ icon.text }}</h6>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
.goes_here {
    padding: 2rem 1rem;
    background-color: #1C1C1C;
}

.icons {
    padding: 3rem 0;
    background-color: #0282F9;

}
</style>