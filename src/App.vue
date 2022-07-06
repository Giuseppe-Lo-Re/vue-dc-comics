<template>
  <div id="app">

    <!-- Header -->
    <PageHeader />

    <!-- Main -->
    <main>
      <SectionContents />
      <SectionLinks />
    </main>

    <!-- Footer -->
    <PageFooter />
  </div>
</template>

<script>
import PageHeader from "./components/PageHeader.vue";
import SectionContents from "./components/SectionContents.vue";
import SectionLinks from "./components/SectionLinks.vue";
import PageFooter from "./components/PageFooter.vue";

export default {
  name: "App",
  components: {
    PageHeader,
    SectionContents,
    SectionLinks,
    PageFooter
  }
}
</script>

<style lang="scss">
@import "./style/common";
</style>
