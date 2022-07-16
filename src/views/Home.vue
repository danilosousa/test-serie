<template>
  <div id="app">
    <Header />    
    <BannerFull />
    <BannerMini />
    <div class="container">
     <section class="novidades">
      <h3>novidades</h3>
     </section>
     <section class="banners__content">
        <div class="banners__content--left">left</div>
        <div class="banners__content--right">right</div>
     </section>
     <section class="destaques">
        <h3>novidades</h3>
     </section>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header/Header.vue';
import Footer from '@/components/Footer/Footer.vue';
import BannerFull from '@/components/BannerFull/BannerFull.vue';
import BannerMini from '@/components/BannerMini/BannerMini.vue';
export default {
  name: 'Home',
  components: {
    Header,
    Footer,
    BannerFull,
    BannerMini,
  }
}
</script>

<style lang="scss">

</style>
