<template>
    <footer>
        <div class="container">

            <!-- Footer Top -->
            <div class="footer-top">

                <!-- Nav Left -->
                <div class="nav-left">

                    <!-- DC COMICS -->
                    <div class="dc-comics-nav">

                        <!-- Title -->
                        <h3>
                            DC COMICS
                        </h3>

                        <!-- List -->
                        <ul>
                            <li 
                                v-for="(link, index) in LinksDcComics"
                                :key="index"
                            >
                                <a :href="link.url">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>

                    <!-- SHOP -->
                    <div class="shop-nav">

                        <!-- Title -->
                        <h3>
                            SHOP
                        </h3>

                        <!-- List -->
                        <ul>
                            <li 
                                v-for="(link, index) in LinksShop"
                                :key="index"
                            >
                                <a :href="link.url">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>

                <!-- Nav Center -->
                <div class="nav-center">

                    <!-- DC -->
                    <div class="dc-nav">

                        <!-- Title -->
                        <h3>
                            DC
                        </h3>

                        <!-- List -->
                        <ul>
                            <li 
                                v-for="(link, index) in LinksDc"
                                :key="index"
                            >
                                <a :href="link.url">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>

                <!-- Nav Right -->
                <div class="nav-rigth">

                    <!-- SITES -->
                    <div class="sites-nav">

                        <!-- Title -->
                        <h3>
                            SITES
                        </h3>

                        <!-- List -->
                        <ul>
                            <li 
                                v-for="(link, index) in LinksSites"
                                :key="index"
                            >
                                <a :href="link.url">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>

                <!-- Image -->
                <div class="img-container">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-bg">
                </div>
            </div>
        </div>

        <!-- Footer Bottom -->
            <div class="footer-bottom">
                <div class="container">

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
            </div>
    </footer>
</template>

<script>
export default {
    name: "PageFooter",
    data() {
        return {
            LinksDcComics: [
               {
                    text: 'Characters',
                    url: '#'
                },
                {
                    text: 'Comics',
                    url: '#'
                },  
                {
                    text: 'Movies',
                    url: '#'
                },
                {
                    text: 'TV',
                    url: '#'
                },
                {
                    text: 'Games',
                    url: '#'
                },
                {
                    text: 'Videos',
                    url: '#'
                },
                {
                    text: 'News',
                    url: '#'
                },
            ],
            LinksShop: [
                {
                    text: 'Shop DC',
                    url: '#'
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#'
                },  
            ],
            LinksDc: [
                {
                    text: 'Terms Of Use',
                    url: '#'
                },
                {
                    text: 'Privacy policy(New)',
                    url: '#'
                },    
                {
                    text: 'Ad Choices',
                    url: '#'
                },
                {
                    text: 'Advertising',
                    url: '#'
                },
                {
                    text: 'Jobs',
                    url: '#'
                },
                {
                    text: 'Subscriptions',
                    url: '#'
                },
                {
                    text: 'Talent Workshops',
                    url: '#'
                },
                {
                    text: 'CPSC Certificates',
                    url: '#'
                },
                {
                    text: 'Ratings',
                    url: '#'
                },
                {
                    text: 'Shop help',
                    url: '#'
                },
                {
                    text: 'Contact Us',
                    url: '#'
                },
            ],
            LinksSites: [
                {
                    text: 'DC',
                    url: '#'
                },
                {
                    text: 'MAD magazine',
                    url: '#'
                }, 
                {
                    text: 'DC Kids',
                    url: '#'
                }, 
                {
                    text: 'DC Universe',
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    url: '#'
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;

    .footer-top {
        display: flex;
        padding: 40px 0;
        position: relative;
        overflow: hidden;

        h3 {
            color: white;
            padding-block: 20px;
        }

        li {

            a {
                text-decoration: none;
                color: $brand_tertiary_color;
                font-size: 12px;
            }
        }

        .nav-center {
            padding-inline: 30px;
        }
        
        .img-container {
            position: absolute;
            top:-100px;
            right:50px;

            img {
                width: 550px;
            }
        }
    }

    .footer-bottom {
        background-color: #303030;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 30px 20px;
        }

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