<template>
  <div id="about" class="container">
    <div class="container__horizontal">
      <div class="container__horizontal__vertical">
        <div class="container__horizontal__vertical--png">
        </div>
      </div>
      <div class="container__horizontal__vertical--right">
        <div>
          <h2 class="animate__animated animate__backInRight animate__delay-2s">
            Hola, ¿Cómo estás?
          </h2>
          <br>
          <div>
            <p class="animate__animated animate__backInRight animate__delay-3s">
              Mi nombre es <strong>Juan</strong>. Me dedico al desarrollo web, más precisamente Front-end. Soy un apasionado desde chico por aprender lo más posible por mi constante necesidad de adquirir nuevos conocimientos en distintas áreas.
            </p>
          </div>
          <br>
          <p class="animate__animated animate__backInRight animate__delay-3s">
            Dado esto empecé a educarme como autodidacta y me considero motivado constantemente para lograr seguir desarrollando mis habilidades, para así crecer profesionalmente como Desarrollador Full-Stack.
          </p>
          <br>
          <p class="animate__animated animate__backInRight animate__delay-3s">
            Ofrezco un <strong>servicio personalizado</strong> y flexible, ya sea por proyecto o con planes mensuales. Según las necesidades de cada persona desde el inicio hasta el final del proyecto. <strong>¡Desde Buenos Aires al mundo!</strong>
          </p>
          <br>
          <p class="animate__animated animate__backInRight animate__delay-3s">
            <strong>Skills </strong> <br>
            HTML | CSS | JavaScript |  Vue.js | Bootstrap | SCSS | BEM | Visual Studio Code | Git | Github | Figma | Gestión por objetivos | Aprendizaje continuo | Creatividad |
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  *{
    margin: 0px;
    padding: 0px;
  }
  .container{
    display:flex;
    flex-direction: column;
    &__horizontal{
      display:flex;
      flex-wrap: nowrap;
      width: 100%;
      background-color: #fff;
      color:#333;
      font-family: 'Poppins';
      &__vertical{
        width: 50%;
        padding: 0px 30px;
        margin: 20px 20px;
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;

        font-size: 13px;
        line-height: 25px;
        text-align: start;
        align-items: center;
        letter-spacing: 0.03em;
        background-image: url('../assets/coding_.svg');
        background-repeat: no-repeat;
        background-position-y: center;
      }
      &__vertical--right{
        width: 50%;
        padding: 0px 30px;
        margin: 20px 20px;
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
        overflow: hidden;
        animation:alternate;

        font-size: 16px;
        line-height: 25px;
        text-align: start;
        align-items: center;
        letter-spacing: 0.03em;
      }
    }

    @media screen and (min-width: 320px) and (max-width: 360px) {
      .container{
        font-size: 12px;

        &__horizontal{
          display:flex;
          flex-flow: row wrap;
          &__vertical {
            width: 100%;
          }
          &__vertical p{
            font-size: 12px;
            padding: 5px;
          }
          &__vertical--png {
            display:flex;
            justify-content: center;
            align-items:center;
            width:250px;
            height:250px;
          }
          &__vertical--png img{
            width:250px;
            height:350px;
          }

          &__vertical--right {
            font-size: 13px;
          }
        }
      }
    }

    @media screen and (min-width: 375px) and (max-width: 480px) {
      .container{
        font-size: 12px;

        &__horizontal{
          display:flex;
          flex-flow: row wrap;
          &__vertical {
            width: 100%;
          }
          &__vertical p{
            font-size: 12px;
            padding: 5px;
          }
          &__vertical--png {
            display:flex;
            justify-content: center;
            align-items:center;
            width:250px;
            height:250px;
          }
          &__vertical--png img{
            width:250px;
            height:350px;
          }

          &__vertical--right {
            font-size: 13px;
          }
        }
      }
    }
  }
</style>

<script>
export default {
  name: 'AboutMe'
}
</script>
