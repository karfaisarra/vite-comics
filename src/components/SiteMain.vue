<script>
import Comics from './Comics.vue'
import Banner from './Banner.vue'
export default {
    name: 'SiteMain',
    components: {
        Banner,
        Comics
    }

}
</script>
<template>
    <main id="site_main">
        <Comics />
        <Banner />

    </main>
</template>

<style lang="scss" scoped>

</style>