<template>
  <div id="service" class="container">
    <div class="parent">
      <div class="div1">
        <div class="card__title">
          <h2>
            Web <br> Development
          </h2>
          <img src="../assets/dev.png" alt="development">
          </div>
            <p>
              Desarrollo de paginas web para impulsar todo tipo y tamaño de empresas.
      Para ello ofrezco soluciones en cada parte del <strong>ciclo de vida</strong> de un sitio web o aplicación: diseño, programación y mejora continua,
      podemos lograr los mejores resultados con las <strong>tecnologías más eficientes</strong>.
            </p>
      </div>
      <div class="div2">
        <div class="card__title">
          <h2>
            E-commerce
          </h2>
          <img src="../assets/Ecommerce.png" alt="e-commerce">
          </div>
          <p>
            ¿Se le ocurrio un <strong>excelente negocio</strong>? ¿Quiere dar <strong>un paso más</strong> alla de su local fisico?
            Podemos impulsar su proyecto con el uso de las más modernas APIs
            con el fin de <strong>llegar a más clientes</strong>, ofrecer informacion de productos y <strong>facilitar el soporte</strong> al departamento de Marketing.
          </p>
      </div>
      <div class="div3">
        <div class="card__title">
        <h2>
          Diseño Responsive
        </h2>
        <img src="../assets/responsive.png" alt="responsive">
        </div>
          <p>
            Diseño de paginas web responsive para que tu emprendimiento pueda ser visualizado desde todo dispositivo.
            En la actualidad una de las partes importantes de un sitio web o aplicación es poder garantizar un correcto     <strong>desempeño</strong> y <strong>visualizacion</strong> donde sea que se lo utilice.
          </p>
      </div>
      <div class="div4">
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
  </div>
</template>

<style lang="scss" scoped>
  .container{
    font-family: 'Poppins';
    display:flex;
    flex-flow: row wrap;
    font-size: 14px;

    .parent {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(5, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 0px;
    max-height: 600px;
  }

  .div1 {
    grid-area: 1 / 2 / 2 / 3;
    margin: 10px 10px;
    text-align: start;
    margin: 10px 10px;
    padding: 10px 10px;
    width: 500px;
    text-align: start;
    background: linear-gradient(90deg, #ECE9E6 0%, #FFFFFF 100%);
    box-shadow: 0px 4px 9px rgba(0, 0, 0, 0.36);

    .card__title{
      display:flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
    }
  }
  .div2 {
    grid-area: 1 / 4 / 2 / 5;
    margin: 10px 10px;
    padding: 10px 10px;
    width: 500px;
    text-align: start;
    background: linear-gradient(90deg, #ECE9E6 0%, #FFFFFF 100%);
    box-shadow: 0px 4px 9px rgba(0, 0, 0, 0.36);
    border-radius: 9px;
    .card__title{
      display:flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
    }
  }
  .div3 {
    grid-area: 2 / 2 / 3 / 3;
    margin: 10px 10px;
    text-align: start;
    margin: 10px 10px;
    padding: 10px 10px;
    width: 500px;
    text-align: start;
    background: linear-gradient(90deg, #ECE9E6 0%, #FFFFFF 100%);
    box-shadow: 0px 4px 9px rgba(0, 0, 0, 0.36);
    .card__title{
      display:flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
    }
  }
  .div4 {
    grid-area: 2 / 4 / 3 / 5;
    margin: 10px 10px;
    text-align: start;
    margin: 10px 10px;
    padding: 10px 10px;
    width: 500px;
    text-align: start;
    background: linear-gradient(90deg, #ECE9E6 0%, #FFFFFF 100%);
    box-shadow: 0px 4px 9px rgba(0, 0, 0, 0.36);
    .card__title{
      display:flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
    }
  }
  }
</style>

<script>
export default {
  name: 'Services'
}
</script>
