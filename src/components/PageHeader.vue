<template>
<header>

    <header-wrapper>
        <!-- Logo -->
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="dc-logo-header">
        </div>

        <nav class="menu">
            <ul>
                <li>
                    link
                </li>

                <li>
                    link
                </li>

                <li>
                    link
                </li>

                <li>
                    link
                </li>

                <li>
                    link
                </li>

                <li>
                    link
                </li>

                <li>
                    link
                </li>

                <li>
                    link
                </li>

                <li>
                    link
                </li>

                <li>
                    link
                </li>
            </ul>
        </nav>
    </header-wrapper>

</header>
</template>

<script>

export default {
    name: "PageHeader",
}
</script>

<style lang="scss" scoped>
// @import './style/variables';
header {
    .header-wrapper {
       display: flex;
       justify-content: space-between;
       // background-color:;
   
       ul {
           display: flex;
       }
    }
    .logo {
       width: 80px;
    }
}
</style>