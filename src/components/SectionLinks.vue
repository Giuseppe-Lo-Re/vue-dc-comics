<template>
    <section>
        
        <ul>
            <li 
                v-for="(link, index) in menuLinks" 
                :key="index"
            >
                <a :href="link.url">

                    <!-- link Image -->
                    <img :src="link.image" :alt="link.text">
                    
                    <!-- link Info -->
                    <div>
                        {{ link.text }}
                    </div>    
                </a>
            </li>
        </ul>
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
                    image: '../assets/img/buy-comics-digital-comics.png',
                    url: '#',
                },
                {
                    text: 'DC MERCHANDISE',
                    image: '../assets/img/buy-comics-merchandise.png',
                    url: '#',
                },
                {
                    text: 'SUBSCRIPTION',
                    image: '../assets/img/buy-comics-subscription.png',
                    url: '#',
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    image: '../assets/img/buy-comics-shop-locator.png',
                    url: '#',
                },
                {
                    text: 'DC POWER VISA',
                    image: '../assets/img/buy-dc-power-visa.png',
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
    background-color: $brand_secondary_color;

    img {
        width: 50px;
    
}
}
</style>