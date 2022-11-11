<script>
import comics from '../components/data/comics.js'
import Comic from './Comic.vue'
export default {
    name: 'Comics',
    data() {
        return {
            comics,
        }
    },
    components: {
        Comic,
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
                <div class="row row-cols-6 g-4">
                    <Comic v-for="comic in comics" :image="comic.thumb" :title="comic.series" />
                    <!--<div class="col" v-for="comic in comics">
                        <img :src="comic.thumb" alt="">
                        <h5>{{ comic.series }}</h5>
                    </div>-->
                </div>
                <div class="btn">
                    <a href="#">Load More</a>
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

            &:hover {
                background-color: white;
                color: #0282F9;
            }
        }
    }
}

.bottom {
    padding: 3rem 0;
    background-color: #1C1C1C;

    .btn {
        padding-top: 2rem;
        width: 100%;
        text-align: center;

        a {
            text-decoration: none;
            color: white;
            padding: 0.5rem 3rem;
            background-color: #0282F9;
            text-transform: uppercase;
            font-weight: 600;

            &:hover {
                background-color: white;
                color: #0282F9;
            }
        }
    }
}
</style>