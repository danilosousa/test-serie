<template>
  <div>
    <nav class="nav">
      <div class="container">
        <ul class="nav__menu">
          <li class="nav__menu--list"><a href="#">Cachorros</a></li>
          <li class="nav__menu--list"><a href="#">Gatos</a></li>
          <li class="nav__menu--list"><a href="#">Passáros</a></li>
          <li class="nav__menu--list"><a href="#">Peixes</a></li>
          <li class="nav__menu--list"><a href="#">Outros Pets</a></li>
          <li class="nav__menu--list"><a href="#">Casa & Jardim</a></li>
          <li class="nav__menu--hamburguer">
            <span></span>
            <span></span>
            <span></span>
          </li>
        </ul>
        
      </div>
    </nav>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .nav {
    background: #8158c5;
    padding: 16px 0;
    &__menu {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 30px;
      &--list {
        display: flex;
        justify-content: space-between;
        a {
          color:#fff;
          text-decoration: none;
          
          font-weight: bold;
          &:hover {
            text-decoration: underline;
          }
        }
      }
      &--hamburguer {
    
        span {
          width: 35px;
          height: 4px;
          background: #fff000;
          display: block;
          margin: 6px 0;
        }
      }
    }
  }
</style>