<template>
  <div id="app">

    <!-- Header -->
    <PageHeader />


    <main>
      <SectionContents />
      <SectionLinks />
    </main>

    <footer>
      <FooterTop />
      <FooterBottom />
    </footer>
    

  </div>
</template>


<script>
import PageHeader from "./components/PageHeader.vue";
import SectionContents from "./components/SectionContents.vue";
import SectionLinks from "./components/SectionLinks.vue";
import FooterTop from "./components/FooterTop.vue";
import FooterBottom from "./components/FooterBottom.vue";

export default {
  name: "App",
  components: {
    PageHeader,
    SectionContents,
    SectionLinks,
    FooterTop,
    FooterBottom
  }
}
</script>


<style lang="scss">
@import "./style/common"
</style>
