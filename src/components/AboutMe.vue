<template>
  <div id="about" class="container">
    <div class="container__horizontal">
      <div class="container__horizontal__vertical">
        <div class="container__horizontal__vertical--png">
        <img src="@/assets/png2.svg" alt="png personal">
        </div>
        <div class="container__horizontal__vertical--info">
          <img src="@/assets/separador1.svg" alt="separador">
          <h2>
            Servicios que brindo
          </h2>
          <p>
            Trabajo por proyecto o con planes mensuales, adaptandome a tus necesidades.
            <br>
            <strong>SKILLS</strong> <br>
            HTML | CSS | JavaScript |  Vue.js | Bootstrap | SCSS | Visual Studio Code | Git | Github | Figma | BEM | GraphQL | REST | Firebase | Gestión por objetivos | Aprendizaje continuo | Creatividad
          </p>
        </div>
      </div>
      <div class="container__horizontal__vertical--right">
        <div>
          <h2 class="animate__animated animate__backInRight animate__delay-1s">
            Hola, ¿Como estás?
          </h2>
          <br>
          <div>
            <p class="animate__animated animate__backInRight animate__delay-2s">
              Mi nombre es <strong>Juan</strong>. Me dedico al desarrollo web, más precisamente Front-end. Soy un apasionado desde chico por aprender lo más posible por mi constante necesidad de adquirir nuevos conocimientos en distintas áreas.
            </p>
          </div>
          <br>
          <p class="animate__animated animate__backInRight animate__delay-2s">
            Dado esto, es que me considero motivado constantemente para lograr seguir desarrollando mis habilidades, y crecer profesionalmente como Desarrollador Full-stack.
          </p>
          <br>
          <p class="animate__animated animate__backInRight animate__delay-3s">
            Ofrezco un <strong>servicio personalizado</strong> y flexible según las necesidades de cada persona desde el inicio hasta el final del proyecto. <strong>Desde Buenos Aires al mundo!</strong>
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
  }
</style>

<script>
export default {
  name: 'AboutMe'
}
</script>
