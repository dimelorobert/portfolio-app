<template>
  <div class="container">
    <div id="portfolio" class="banner">
      <div class="banner__info">
        <h2>
          ¿Querés que trabajemos juntos?
        </h2>
        <a href="#contact">
          HABLEMOS
        </a>
      </div>
    </div>
    <div class="projects">
      <div class="projects__info">
        <p>
          <strong>Creo proyectos fuertes, con identidad.</strong>
        </p>
      </div>
      <br>
      <div class="projects__works">
        <div class="card">
          <img src="@/assets/Birds2.png" alt="work1">
        </div>
        <div class="card">
          <img src="@/assets/TanzeeCo.png" alt="work2">
        </div>
        <div class="card">
          <img src="@/assets/Skylanding.png" alt="work3">
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .container{
    font-family: 'Poppins';

    .banner{
      background-image: url('../assets/banner2.svg');
      background-size: cover;
      height: 40vh;
      display:flex;
      justify-content: center;
      align-items: center;

      &__info{
        display:flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
      }
      &__info h2{
        color: #fff;
        margin: 20px;
        font-weight: 300;
        font-size: 30px;
        line-height: 45px;
      }
      &__info a{
        text-decoration: none;
        color: #fff;
        font-family: 'red rose';
        display:flex;
        justify-content: center;
        padding: 15px 15px;
        width: 25%;
        background: #4EBFFE;
        border-radius: 9px;
      }
      &__info a:hover{
        background: #87d5ec;
      }
    }

    .projects{
      display:flex;
      flex-direction: column;
      &__info{
        margin: 30px;
        width: 305px;
        display:flex;
        flex-direction: column;
        justify-content: flex-start;
        text-align: start;
        border-top: 2px solid #1DAEEC;
      }
      &__works{
        display:flex;
        justify-content: center;
        align-items: center;

        .card{
          background: linear-gradient(90deg, #ECE9E6 0%, #FFFFFF 100%);
          box-shadow: 0px 4px 11px rgba(0, 0, 0, 0.5);
          border-radius: 3px;
          width: 417px;
          height: 300px;
          margin: 20px;

          display:flex;
          justify-content: space-evenly;
          align-items: center;
        }
        .card:hover{
          background: linear-gradient(180deg,  #ECE9E6 0%, rgba(21, 9, 9, 0) 120%), #3f92df;
          transition: linear 350ms;
        }
        .card img{
          width: 80%;
          border-radius: 5px;
        }
      }
    }
  }
</style>

<script>
export default {
  name: 'Projects'
}
</script>
