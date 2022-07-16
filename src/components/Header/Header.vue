<template>
  <div>
    <div class="container">
      <header class="header">
        <div class="header__search">
           <input type="text" class="header__search--input" placeholder="Pesquisar" >
           <button type="submit" class="header__search--submit"><i class=""></i></button>           
        </div>
        <div class="header__logo">
          <img src="../../assets/logo-pet-store.png" alt="">
        </div>
        <div class="header__infos">
          <ul>
            <li><img src="../../assets/icon-login.png" alt=""></li>
            <li><img src="../../assets/icon-carrinho.png" alt=""></li>          
          </ul>
        </div>
      </header>

    </div>
     <Nav />
  </div>
</template>

<script>
import Nav from '../Nav/Nav';

export default {
  components: {
    Nav
  }
}
</script>

<style lang="scss">

  .header {
    width: 100%;
    padding: 20px 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
    &__search {
      width: 30%;
      &--input {
        width: 65%;
        border: 1px solid #7f7f7f;        
        padding: 5px;
        height: 20px;
        border-radius: 5px 0 0 5px;
        outline: none;
        color: #9DBFAF;
      }
      &--submit{
        width: 40px;
        height: 28px;
        border: none;
        background: none;
        text-align: center;
        background: #fff;
        color: #fff;
        border-radius: 0 5px 5px 0;
        cursor: pointer;
        /* font-size: 20px; */
        position: relative;
        top: 11px;
        left: -43px;

        i {
          background: url('../../assets/icon-lupa.png') no-repeat;
          width: 29px;
          height: 29px;
          display: inline-block;
          background-size: 90%;
        }
      }
    }

    &__logo {
      width: 50%;
      text-align: center;
    }
    &__infos {
      width: 20%;
      display: flex;
      justify-content: flex-end;
      ul{
        display: flex;
        li {
          padding: 0 5px;
        }
      }
    }
  
  }
</style>