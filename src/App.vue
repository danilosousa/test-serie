<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
*{
  padding: 0;
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  //text-align: center;
  color: #2c3e50;
}

  ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }
.container {
    width: 100%;  
    margin-right: auto;
    margin-left: auto;
}

@media (min-width: 576px) {
  .container {
      max-width: 540px;
  }
}
@media (min-width: 768px) {
  .container {
      max-width: 720px;
  }
}
@media (min-width: 992px) {
  .container {
      max-width: 960px;
  }
}

@media (min-width: 1200px) {
  .container {
      max-width: 1140px;
  }
}


@media (min-width: 1400px) {
  .container {
      max-width: 1320px;
  }
}

#nav {
  padding: 30px;
}
</style>
