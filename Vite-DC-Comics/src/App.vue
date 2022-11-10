<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteMaine from './components/SiteMain.vue';
export default {
  name: 'Vite-DC-Comics',
  components: {
    SiteHeader,
    SiteMaine,
  }
}
</script>
<template>
  <SiteHeader></SiteHeader>
  <!-- /#site_header -->
  <SiteMaine></SiteMaine>
  <!-- /#site_main -->
  <footer id="site_footer"></footer>
  <!-- /#site_footer -->
</template>
<style>

</style>