<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteMaine from './components/SiteMain.vue';
import SiteFooter from './components/SiteFooter.vue';

export default {
  name: 'Vite-DC-Comics',
  components: {
    SiteHeader,
    SiteMaine,
    SiteFooter,
  }
}
</script>
<template>
  <SiteHeader></SiteHeader>
  <!-- /#site_header -->
  <SiteMaine></SiteMaine>
  <!-- /#site_main -->
  <SiteFooter></SiteFooter>
  <!-- /#site_footer -->
</template>
<style>

</style>