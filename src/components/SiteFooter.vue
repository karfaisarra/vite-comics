<script>
export default {
    name: 'SiteFooter'
}
</script>
<template>
    <footer id="site_footer">
        <div class="top">
            <div class="container">
                <div class="row">
                    <div class="col-5">
                        <div class="row">
                            <div class="col">
                                <h4 class="text-uppercase text-white">dc comics</h4>
                                <ul class="list-unstyled">
                                    <li><a href="#">Characters</a></li>
                                    <li><a href="#">Comics</a></li>
                                    <li><a href="#">Movies</a></li>
                                    <li><a href="#">TV</a></li>
                                    <li><a href="#">Games</a></li>
                                    <li><a href="#">Videos</a></li>
                                    <li><a href="#">News</a></li>
                                </ul>
                                <h4 class="text-uppercase text-white">Shop</h4>
                                <ul class="list-unstyled">
                                    <li><a href="#">Shop DC</a></li>
                                    <li><a href="#">Shop DC Collectibles</a></li>
                                </ul>
                            </div>
                            <div class="col">
                                <h4 class="text-uppercase text-white">dc</h4>
                                <ul class="list-unstyled">
                                    <li><a href="#">Terms Of Use</a></li>
                                    <li><a href="#">Privacy policy (New)</a></li>
                                    <li><a href="#">Ad Choices</a></li>
                                    <li><a href="#">advertising</a></li>
                                    <li><a href="#">Job</a></li>
                                    <li><a href="#">Subscription</a></li>
                                    <li><a href="#">Talent Workshops</a></li>
                                    <li><a href="#">CPSC Certificates</a></li>
                                    <li><a href="#">Ratings</a></li>
                                    <li><a href="#">Shop Help</a></li>
                                    <li><a href="#">Contact Us</a></li>
                                </ul>
                            </div>
                            <div class="col">
                                <h4 class="text-uppercase text-white">sites</h4>
                                <ul class="list-unstyled">
                                    <li><a href="#">DC</a></li>
                                    <li><a href="#">MAD Magazine</a></li>
                                    <li><a href="#">DC Kids</a></li>
                                    <li><a href="#">DC Universe</a></li>
                                    <li><a href="#">DC Power Visa</a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="col-7 text-end">
                        <img height="400px" src="../assets/img/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom">
            <div class="container">
                <div class="row align-items-center">
                    <div class="col-6">
                        <div class="my_btn text-uppercase "><a href="#">sing-up now !</a></div>
                    </div>
                    <div class="col d-flex align-items-center">
                        <span class="text-uppercase">follow us</span>
                        <img src="../assets/img/footer-facebook.png" alt="">
                        <img src="../assets/img/footer-twitter.png" alt="">
                        <img src="../assets/img/footer-youtube.png" alt="">
                        <img src="../assets/img/footer-pinterest.png" alt="">
                        <img src="../assets/img/footer-periscope.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </footer>

</template>
<style lang="scss" scoped>
.top {
    background-image: url(../assets/img/footer-bg.jpg);
    height: 400px;

    h4 {
        margin: 1rem 0;
    }

    a {
        text-decoration: none;
        color: gray;
    }
}

.bottom {
    background-color: #303030;

    .my_btn {
        margin: 2.5rem 0;

        a {
            text-decoration: none;
            color: white;
            border: 2px solid #0282F9;
            padding: 0.75rem;

        }
    }

    .col {
        span {
            margin: 0 1rem;
            color: #0282F9;
            font-size: 20px;
            font-weight: bold;
        }

        img {
            margin-right: 1.5rem;
        }
    }
}
</style>