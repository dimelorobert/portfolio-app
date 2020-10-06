<template>
  <div id="app">
    <div id="nav">
      <div class="nav--logo">
        <p class="name">
          Juan Loyola
        </p>
        <br>
        <p class="title">
          Front-end developer
        </p>
      </div>
      <div>
        <a href="#nav">Inicio</a>
        <a href="#about">Sobre mi</a>
        <a href="#service">Servicios</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#contact">Contacto</a>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
*{
  margin:0px;
  padding: 0px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
}

#nav {
  background: rgb(57, 58, 59);
  display:flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 50px;

  font-family: 'Poppins';
  color:#fff;
  position: sticky;
  top: 0;

  .name {
    font-family: 'red rose';
  }

  .title {
    font-size: 14px;
    margin-top: -15px;
  }
  a {
    color: #fff;
    text-decoration: none;
    margin:10px;
  }
  a:hover {
    color: rgb(233, 219, 20);
  }
}
</style>
