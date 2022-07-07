<template>
    <section>

        <!-- Jumbotron -->
        <div class="jumbotron">
        </div>

        <div class="container">

            <!-- Title -->
            <div class="title position">
                CURRENT SERIES
            </div>

            <!-- Products List -->
            <div class="products-list">
                <ProductCard 
                    v-for="(product,index) in products" 
                    :key="index" 
                    :productDetails="product" 
                />
            </div>

            <!-- Load More -->
            <div class="wrapper">
                <div class="title padding-cursor">
                    LOAD MORE
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import productsJson from "../assets/dc-comics.json";
import ProductCard from "./ProductCard.vue";


export default {
    name: "SectionContents",
    components: {
        ProductCard
    },
    data() {
        return {
            products: productsJson
        };
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
@import '../style/common';

section {
    background-color: black;

    .jumbotron {
        background-image: url(../assets/img/jumbotron.jpg);
        background-position: top;
        height: 400px;
        position: relative;
    }

    .title {
        color: white;
        background-color: $brand_secondary_color;
        border: 1px solid $brand_secondary_color;
        display: inline;
        padding: 10px 20px;
        font-size: 18px;
        font-weight: bold;
        
        &.position {
            position: absolute;
            bottom: 242px;
            left: 60px;
        }

        &.padding-cursor {
            padding: 10px 80px;
            cursor: pointer;
        }
    }
    
    .products-list {
        color: white;
        display: flex;
        flex-wrap: wrap;
    }

    .wrapper {
        text-align: center;
        padding: 50px;
    }
}  
</style>