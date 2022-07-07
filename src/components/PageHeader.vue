<template>
<header>
    <div class="container">
        <div class="header-wrapper">

            <!-- Logo -->
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="dc-logo-header">
            </div>

            <!-- Menu -->
            <div class="menu">
                <ul>
                    <li 
                        v-for="(link, index) in menuLinks" 
                        :key="index" 
                        :class="{ 'current' : link.current}"
                    >
                        {{ link.text }}
                    </li>
                </ul>
            </div>
        </div>
    </div>

</header>
</template>

<script>
export default {
    name: "PageHeader",
    data() {
        return {
            menuLinks: [
               {
                    text: 'CHARACTERS',
                    current: false
                },
                {
                    text: 'COMICS',
                    current: true
                },  
                {
                    text: 'MOVIES',
                    current: false
                },
                {
                    text: 'TV',
                    current: false
                },
                {
                    text: 'GAMES',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    current: false
                },
                {
                    text: 'VIDEOS',
                    current: false
                },
                {
                    text: 'FANS',
                    current: false
                },
                {
                    text: 'NEWS',
                    current: false
                },
                {
                    text: 'SHOP',
                    current: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

header {
    background-color: white;
    
    .header-wrapper {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .logo {
           width: 80px;
           cursor: pointer;
        }
    
        ul {
            display: flex;
            padding-right: 50px;

            li {
                margin: 0 15px;
                line-height: 94px;
                text-decoration: none;
                color: $brand_main_color;
                font-size: 13px;
                font-weight: bold;
                cursor: pointer;

                &.current {
                color: $brand_secondary_color;          
                border-bottom: 1px solid $brand_secondary_color;
                border-bottom-width: 5px;
                }
            }
        }       
    }
}
</style>