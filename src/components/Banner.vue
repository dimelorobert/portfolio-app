<template>
  <div class="container">
    <div class="container__info">
      <div class="container__info--name">
        <h2 class="name">
          Juan Loyola
        </h2>
        <p class="container__info--title">
          Front-end Developer
        </p>
      </div>
      <div class="container__btn">
        <a class="container__btn--portfolio" href="#portfolio">
          Mi Portfolio
        </a>
        <a class="container__btn--contacto" href="#contact">
          Contactame
        </a>
      </div>
      <div class="container__social">
        <a href="https://www.linkedin.com/in/juan-loyola-81a611162/" target="_blank">
          <img src="@/assets/Linkedin.png" alt="LinkedIn">
        </a>
        <a href="https://github.com/JuanLoyola" target="_blank">
          <img src="@/assets/Github.png" alt="Github">
        </a>
        <a href="https://www.behance.net/Loyolajuan" target="_blank">
          <img src="@/assets/Behance.png" alt="BeHance">
        </a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .container{
    background-image: url('../assets/banner1.svg');
    background-repeat: no-repeat;
    background-position-y: center;
    color: #fff;
    font-family: 'Poppins';
    background-size: 100%;
    display:block;

    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;

    a{
      text-decoration: none;
      color: #fff;
    }
    a img{
      width: 50px;
      margin: 20px;
    }

    &__info{
      margin-left: 80px;
      text-align: start;
    }

    &__info--name{
      font-family: 'Poppins';
      font-style: normal;
      font-weight: normal;
      font-size: 46px;
      line-height: 49px;
    }
    .name {
      border-right: solid 3px rgba(0,255,0,.75);
      white-space: nowrap;
      overflow: hidden;
      font-size: 46px;
      color: #fff;
    }
    .name {
      animation: animated-text 2s steps(29,end) 1s 1 normal both,
      animated-cursor 600ms steps(29,end) infinite;
    }

    @keyframes animated-text{
      from{width: 0;}
      to{width: 270px;}
    }

    @keyframes animated-cursor{
      from{
        border-right-color: rgba(255,255,255,.9);
      }
      to{
        border-right-color: transparent;
      }
    }

    &__info--title{
      font-style: normal;
      font-weight: 300;
      font-size: 16px;
      line-height: 24px;
    }
    &__btn{
      padding: 20px 0px;
    }
    &__btn--portfolio{
      border: 1px solid #7389E1;
      border-radius: 2px;
      padding: 10px 10px;
      margin-right: 30px;
    }
    &__btn--portfolio:hover{
      background-color: rgba(189, 186, 186, 0.808)
    }
    &__btn--contacto{
      border: 1px solid #94E2FB;
      border-radius: 3px;
      padding: 10px 10px;
      margin-right: 30px;
    }
    &__btn--contacto:hover{
      background-color: rgba(189, 186, 186, 0.808)
    }
    &__social a img{
      width: 25px;
    }

    @media screen and (max-width: 480px) {
      .container{
        background-size: 100%;
        margin: 0px;
        padding: 0px;

        &__name{
          display:flex;
          flex-direction: row;
        }
      }
      .container__info--name p {
        font-size: 10px;
        display:flex;
      }

      .container__info--name h2{
        font-size: 1rem;
      }

      .name {
        animation: animated-text 2s steps(29,end) 1s 1 normal both,
        animated-cursor 600ms steps(29,end) infinite;
      }

      @keyframes animated-text{
        from{
          width: 0;
        }
        to{
          width: 93px;
        }
      }

      @keyframes animated-cursor{
      from{
        border-right-color: rgba(255,255,255,.9);
        height: 35px;
      }
      to{
        border-right-color: transparent;
        height: 35px;
      }
    }

      .container__btn--portfolio{
        width: 10%;
        font-size: 8px;
      }

      .container__btn--contacto{
        width: 10%;
        font-size: 8px;
      }

      .container__social{
        display:flex;
        flex-direction: row;
      }

      .container__social img{
        width: 19px;
      }
    }
  }
</style>

<script>
export default {
  name: 'Banner'
}
</script>
