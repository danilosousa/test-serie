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
     <section class="list__destaques">
        <h3>novidades</h3>
        <ul class="product__list">
          <li class="product__list--item" v-for="item in novidades" :key="item.id">
            <small class="product__list--item--flag" v-if="item.discount">{{item.discount}}% OFF </small>
            <span class="product__list--item--image">
              <img :src="require(`../assets/${item.urlImage}`)" />          
            </span>
            <p class="product__list--item--description">{{item.description}}</p>
            <p class="product__list--item--price">R$ {{item.price}}</p>
            <p class="product__list--item--installments" v-if="item.installments">Ou 10x de R$ {{item.installments}}</p>
          </li>
        </ul>
        
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

const arrNovidades = [
  {"id":1, urlImage: 'imagem-url-procudct.png',"description":"amet consectetur, adipisicing","price":900.00,"installments": 90.00,"discount": 20},
  {"id":2, urlImage: 'imagem-url-procudct.png',"description":"Placeat et est asperiores","price":99.99,"installments": 90.00,},
  {"id":3, urlImage: 'imagem-url-procudct.png',"description":"aliquam nulla rerum fugiat adipisci","price":99.99,"installments": 90.00, "discount": 30},
  {"id":4, urlImage: 'imagem-url-procudct.png', "description":"debitis doloremque in magnam","price":60.99,"installments": 90.00,},
]
export default {
  name: 'Home',
  components: {
    Header,
    Footer,
    BannerFull,
    BannerMini,
  },
  data(){
    return {
      novidades: arrNovidades
    }
  }
}
</script>

<style lang="scss">
  .product__list {
    display: flex;
    &--item {      
      width: 25%;
      display: flex;
      flex-direction: column;
      position: relative;
      &--image {
        img {
          width: 90%;
        }
      }
      &--flag{     
        position: absolute;
        left: 0;
        right: 0;
        top: 30px;
        font-size: 20px;
        color: #fff;
        background: #8158c5;
        font-size: 14px;
        width: 20%;
        text-align: center;
        padding: 10px;       
      }
      &--description{
        font-size: 18px;
        margin-top: 10px;
        text-align: center;
        
      }
      &--price{
        margin: 10px 0;
        text-align: center;
      }
      &--installments{
        text-align: center;
      }
    }
  }
</style>
