<template>
  <div class="container">
    <div class="container__info">
      <div class="container__info--name">
        <h2 class="name">
          Juan Loyola
        </h2>
        <p class="container__info--title" v-html="$t('banner.title')">
        </p>
      </div>
      <div class="container__btn">
        <a class="container__btn--portfolio" href="#portfolio">
            {{ $t ('banner.portfolio') }}
        </a>
        <a class="container__btn--contacto" href="#contact">
            {{ $t ('banner.contact') }}
        </a>
      </div>
      <div class="container__social">
        <a href="https://www.linkedin.com/in/juan-loyola-81a611162/" target="_blank">
          <img src="@/assets/linkedin2.png" alt="LinkedIn">
        </a>
        <a href="https://github.com/JuanLoyola" target="_blank">
          <img src="@/assets/Github2.png" alt="Github">
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
    background: #f1f1f1;
    background-image: url('../assets/sample2.png');
    background-repeat: no-repeat;
    background-position-y: bottom;
    background-position: center;
    color: #333;
    font-family: 'Poppins';
    background-size: 100% cover;
    height: 250px;
    display:block;
    box-shadow: 3px 3px 12px #333;

    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;

    .important{
      color: #f79a83;
      font-weight: bold;
    }

    a{
      text-decoration: none;
      color: #333;
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
      color: #333;
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
        border-right-color: rgba(48, 47, 47, 0.9);
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
      border: 2px solid #7389E1;
      border-radius: 5px;
      padding: 10px 10px;
      margin-right: 30px;
    }
    &__btn--portfolio:hover{
      background-color:#7389E1;
      color: #fff;
      transition: linear 300ms;
    }
    &__btn--contacto{
      border: 2px solid #7389E1;
      border-radius: 5px;
      padding: 10px 10px;
      margin-right: 30px;
    }
    &__btn--contacto:hover{
      background-color:#7389E1;
      color: #fff;
      transition: linear 300ms;
    }
    &__social a img{
      width: 25px;
    }
  }

  @media screen and (min-width: 320px) and (max-width: 1150px) {
    .container{
      display:flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: flex-start;

      background-repeat: no-repeat;
      background-position-y: center;
      background-position: right;
      background-size: 55%;

      &__info{
        justify-content:flex-start;
        align-content: flex-start;
        margin-left: 5px;
      }
      .container__info--name h2{
        font-size:1rem;
      }
      .container__info--name p {
        font-size: 10px;
        display:flex;
      }
      @keyframes animated-text{
        from{
          width: 0;
        }
        to{
          width: 110px;
        }
      }

      @keyframes animated-cursor{
      from{
        border-right-color: rgba(61, 59, 59, 0.9);
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

<script src="FadeIn.js"></script>

<script>
export default {
  name: 'Banner'
}
</script>
