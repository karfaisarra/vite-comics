<script>
import comics from '../components/data/comics.js'
export default {
    name: 'Comics',
    data() {
        return {
            comics: comics,
        }
    }
}
</script>
<template>
    <section class="">
        <div class="goes_here">
            <div class="top container">
                <a href="#">current series</a>
            </div>
        </div>
        <div class="bottom">
            <div class="container">
                <div class="row row-cols-6">
                    <div class="col" v-for="comic in comics">
                        <img :src="comic.thumb" alt="">
                        <h4>{{ comic.series }}</h4>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
.goes_here {
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-repeat: no-repeat;

    .top {
        height: 100%;
        position: relative;

        a {
            text-decoration: none;
            color: white;
            background-color: #0282F9;
            padding: 0.5rem 1rem;
            text-transform: uppercase;
            font-weight: 600;
            align-items: flex-end;
            position: absolute;
            bottom: -15px;
            left: 0;
        }
    }
}

.bottom {
    height: 400px;
    background-color: #1C1C1C;
}
</style>