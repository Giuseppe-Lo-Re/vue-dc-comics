<template>
    <section>
        <div class="container">
            <ul>

                <!-- Links -->
                <li 
                    v-for="(link, index) in menuLinks" 
                    :key="index"
                >
                    <a :href="link.url">

                        <!-- link Image -->
                        <img :src="link.image" :alt="link.text">
                        
                        <!-- link Info -->
                        <div class="text">
                            {{ link.text }}
                        </div>    
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: "SectionLinks",
    data() {
        return {
            menuLinks: [
                {
                    text: 'DIGITAL COMICS',
                    image: require('../assets/img/buy-comics-digital-comics.png'),
                    url: '#',
                },
                {
                    text: 'DC MERCHANDISE',
                    image: require('../assets/img/buy-comics-merchandise.png'),
                    url: '#',
                },
                {
                    text: 'SUBSCRIPTION',
                    image: require('../assets/img/buy-comics-subscriptions.png'),
                    url: '#',
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    image: require('../assets/img/buy-comics-shop-locator.png'),
                    url: '#',
                },
                {
                    text: 'DC POWER VISA',
                    image: require('../assets/img/buy-dc-power-visa.svg'),
                    url: '#',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

section {
    display: flex;
    justify-content: center;
    background-color: $brand_secondary_color;

    img {
        width: 55px;
        height: 63px;
    
    }

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    li {
        padding: 50px 30px ;
        
        a {
            display: flex;
            align-items: center;
            text-decoration: none;
            color: white;

            .text {
                padding-left: 10px;
                font-size: 14px;
            }
        }
    }
}
</style>