<template>
    <footer>
        <div class="container">
            <!-- Footer Top -->
            <div class="footer-top">

                <!-- List -->
                <div class="list">
                    <ul>
                        <li class="title-list">
                            DC COMICS
                        </li>

                        <li>
                            <a href="#">
                                Characters
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Comics
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Movies
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                TV
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Games
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Videos
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                News
                            </a>
                        </li>

                        <li class="title-list">
                            SHOP
                        </li>

                        <li>
                            <a href="#">
                                Shop DC
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Shop DC Collectibles
                            </a>
                        </li>

                    </ul>
                </div>

                <!-- List -->
                <div class="list">
                    <ul>
                        <li class="title-list">
                            DC
                        </li>

                        <li>
                            <a href="#">
                                Terms Of Use
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Privacy policy(New)
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Ad Choices
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Advertising
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Jobs
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Subscriptions
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Talent Workshops
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                CPSC Certificates
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Ratings
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Shop help
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                Contact Us
                            </a>
                        </li>

                    </ul>
                </div>

                <!-- List -->
                <div class="list">
                    <ul>
                        <li class="title-list">
                            SITES
                        </li>

                        <li>
                            <a href="#">
                                DC
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                MAD magazine
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                DC Kids
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                DC Universe
                            </a>
                        </li>

                        <li>
                            <a href="#">
                                DC Power Visa
                            </a>
                        </li>
                    </ul>
                </div>

                <!-- Image -->
                <div class="img-container">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-bg">
                </div>
            </div>
        </div>

        <!-- Footer Bottom -->
            <div class="footer-bottom">

                <!-- Button CTA -->
                <a href="#" class="btn">
                    SIGN-UP NOW!
                </a>
                
                <!-- Socials -->
                <div class="social">

                    <!-- Follow us -->
                    <div class="follow-us">
                        FOLLOW US
                    </div>

                    <!-- Social Icons -->
                    <div class="icons">
                        <ul>
                            <li>
                                <!-- Facebook -->
                                <a href="#">
                                    <img src="../assets/img/footer-facebook.png" alt="Facebook">
                                </a>
                            </li>

                            <li>
                                <!-- Twitter -->
                                <a href="#">
                                    <img src="../assets/img/footer-twitter.png" alt="Twitter">
                                </a>
                            </li>

                            <li>
                                <!-- Youtube -->
                                <a href="#">
                                    <img src="../assets/img/footer-youtube.png" alt="Youtube">
                                </a>
                            </li>

                            <li>
                                <!-- Pinterest -->
                                <a href="#">
                                    <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
                                </a>
                            </li>

                            <li>
                                <!-- Periscope -->
                                <a href="#">
                                    <img src="../assets/img/footer-periscope.png" alt="Periscope">
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>

    </footer>
</template>

<script>

export default {
    name: "PageFooter",
}
</script>v

<style lang="scss" scoped>
@import '../style/variables';

footer {
    background-image: url(../assets/img/footer-bg.jpg);
    .footer-top {
        display: flex;
        padding: 40px 0;
        position: relative;
        overflow: hidden;

        .list {
            padding: 0 20px;
        }
        li {
            a {
                text-decoration: none;
                color: $brand_tertiary_color;
                font-size: 12px;
            }
        }
        .title-list {
            font-weight: bold;
            color: white;
            padding: 20px 0;
        }
        .img-container {
            position: absolute;
            top:-100px;
            right:100px;

            img {
                width: 550px;
            }
        }
    }
    .footer-bottom {
        background-color: #303030;
        height: 80px;
        display: flex;
        justify-content: space-around;
        align-items: center;

        .btn {
            border: 2px solid $brand_secondary_color;
            text-decoration: none;
                color: white;
                padding: 10px 20px;
        }

        .social {
            display: flex;
            align-items: center;

            .follow-us {
                color: $brand_secondary_color;
                font-size: 18px;
                font-weight: bold;
                padding-right: 20px;
            }

            ul {
                display: flex;

                li {
                    margin: 0 10px;
                }



            }
            
        }
    }
}
</style>