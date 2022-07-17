<template>
  <div>
    <section class="banner__mini">
      <div class="container">
        <ul class="banner__mini--list">
          <li class="banner__mini--list--racoes">
            <img src="../../assets/mini-banner-01.png" alt="">
          </li>
          <li class="banner__mini--list--brinquedos">
            <img src="../../assets/mini-banner-01.png" alt="">
          </li>
          <li class="banner__mini--list--acessorioss">
            <img src="../../assets/mini-banner-01.png" alt="">
          </li>
        </ul>
      </div>
    </section>
    
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .banner__mini {
    background: #ffa200;
    padding: 20px 0;
    &--list {
      display: flex;
      align-items: center;
      justify-content: space-between;
      width: 100%;
      li {
        margin: 0 10px;
      }
    }
  }
</style>