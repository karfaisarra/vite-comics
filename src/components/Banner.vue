<script>
export default {
    name: 'Banner',
    data() {
        return {
            icons: [
                {
                    image: 'buy-comics-digital-comics.png',
                    title: 'digital comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    title: 'dc merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    title: 'subscription'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    title: 'comic shop locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    title: 'dc power visa'
                },
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    }

}
</script>
<template>
    <section class="icons">
        <div class="container">
            <div class="row">
                <div class="col d-flex align-items-center" v-for="icon in icons">
                    <div class="logo">
                        <img :src="getImageUrl(icon.image)" alt="">
                    </div>
                    <div class="description ps-3">
                        <h6 class="text-uppercase text-white">{{ icon.title }}</h6>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
.icons {
    padding: 3rem 0;
    background-color: #0282F9;
}
</style>