<template>
  <div id="service" class="container">
    <div class="container__card">
      <div class="card__title">
        <h2>
          Web <br> Development
        </h2>
        <img src="../assets/dev.png" alt="development">
      </div>
      <p>
        Desarrollo de páginas web para impulsar todo tipo y tamaño de empresas.
        Para ello ofrezco soluciones en cada parte del <strong>ciclo de vida</strong> de un sitio web o aplicación: diseño, programación y mejora continua,
        podemos lograr los mejores resultados con las <strong>tecnologías más eficientes</strong>.
      </p>
    </div>
    <div class="container__card">
      <div class="card__title">
        <h2>
          E-commerce
        </h2>
        <img src="../assets/Ecommerce.png" alt="e-commerce">
      </div>
      <p>
        ¿Se le ocurrió un <strong>excelente negocio</strong>? ¿Quiere dar <strong>un paso más</strong> alla de su local físico?
        Podemos impulsar su proyecto con el uso de las más modernas APIs
        con el fin de <strong>llegar a más clientes</strong>, ofrecer información de productos y <strong>facilitar el soporte</strong> al departamento de Marketing.
      </p>
    </div>
    <div class="container__card">
      <div class="card__title">
        <h2>
          Diseño Responsive
        </h2>
        <img src="../assets/responsive.png" alt="responsive">
      </div>
      <p>
        Diseño de paginas web responsive para que tu emprendimiento pueda ser visualizado desde todo dispositivo.
        En la actualidad una de las partes importantes de un sitio web o aplicación es poder garantizar un correcto <strong>desempeño</strong> y <strong>visualización</strong> donde sea que se lo utilice.
      </p>
    </div>
    <div class="container__card">
      <div class="card__title">
        <h2>
          ¿Necesita algo más?
        </h2>
        <img src="../assets/design.png" alt="design">
      </div>
      <p>
        Si usted es el tipo de cliente donde día a día se le ocurren nuevas formas de impulsar su negocio o simplemente encuentra antiguo su sitio web actual, puede contactarme para hablar sobre sus ideas o proyectos que tiene en mente para llevar el trabajo en conjunto y mostrarle al mundo esa <strong>gran idea suya</strong>.
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .container{
    font-family: 'Poppins';
    display:flex;
    flex-flow: row wrap;
    font-size: 14px;

    &__card{
      display:flex;
      justify-content: space-around;
      flex-direction: column;
      width: 40%;
      margin: 10px 50px;
      background: linear-gradient(90deg, #ECE9E6 0%, #FFFFFF 100%);
      box-shadow: 0px 4px 9px rgba(0, 0, 0, 0.36);
      border-radius: 9px;

      font-family: 'Poppins';
      font-size: 14px;
      line-height: 21px;
      padding: 10px 10px;
      align-items: center;
      color: #333333;
      text-align: start;

      .card__title{
        display:flex;
        width: 100%;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        text-align: start;
      }
    }
  }
</style>

<script>
export default {
  name: 'Services'
}
</script>
