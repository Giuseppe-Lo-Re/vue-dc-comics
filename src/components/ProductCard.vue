<template>
    <div class="product-card-container">
        <div class="product-card">

            <!-- Image -->
            <div class="img-wrapper">
                <img :src="productDetails.thumb" :alt="productDetails.series">
            </div>

            <!-- Title -->
            <div class="title">
                {{ productDetails.series }}
            </div>
        </div>

    </div>
</template>

<script>
export default {
    name: "ProductCard",
    props: {
        productDetails: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common';

.product-card-container {
    
    width: calc((100% / 6));
    padding-top: 50px;
    
    .product-card {

        .img-wrapper {
            width: 200px;
            height: 200px;
            overflow: hidden;

            img {
                padding: 10px;
            }
        }

        .title {
            color: white;
            font-size: 14px;
            text-transform: uppercase;
            padding: 15px 10px 30px 10px;
        }
    }
}

</style>