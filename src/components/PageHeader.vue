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
                        class="current"
                        >

                        <a :href="link.url">
                        {{ link.text }}
                        </a>

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
                    url: '#',
                    current: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: true
                },  
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false
                    
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
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
    .header-wrapper {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px 0;

        .logo {
           width: 80px;
        }
    
        ul {
            display: flex;

            li {
                padding: 0 20px;

                a {
                    text-decoration: none;
                    color: $brand_main_color;
                    font-size: 12px;
                    font-weight: bold;
                }
            }
        }
    }       
}
.current {
        color: $brand_secondary_color; 
    }
</style>