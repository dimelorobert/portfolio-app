<template>
  <div id="service" class="container">
    <div class="container__card" v-for="(item, index) in services.info[0].variants" :key="index">
      <div class="card__title">
        <h2>
          {{item.name}}
        </h2>
        <img :src="item.image" alt="project">
      </div>
      <p>{{item.text}}</p>
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
      .card__title img{
        width: 15%;
      }
    }
  }
    @media screen and (min-width:320px) and (max-width: 1080px){
      .container{
        width: 100%;
        &__card{
        width: 100%;
      }
      .card__title{
        font-size: 1rem;
        margin-bottom: 25px;
      }
        .card__title img{
        width:50px;
        height:50px;
      }
      }
    }
</style>

<script>
export default {
  name: 'Services',
  data () {
    return {
      services: {
        info: [
          {
            variants: [
              {
                name: 'Web Development',
                image: 'https://i.imgur.com/yZevfRF.png',
                text: 'Desarrollo de páginas web para impulsar todo tipo y tamaño de empresas. Para ello ofrezco soluciones en cada parte del ciclo de vida de un sitio web o aplicación: diseño, programación y mejora continua, podemos lograr los mejores resultados con las tecnologías más eficientes.'
              },
              {
                name: 'E-commerce',
                image: 'https://i.imgur.com/M0UoXXG.png',
                text: '¿Se le ocurrió un excelente negocio? ¿Quiere dar un paso más alla de su local físico? Podemos impulsar su proyecto con el uso de las más modernas APIs con el fin de llegar a más clientes, ofrecer información de productos y facilitar el soporte al departamento de Marketing.'
              },
              {
                name: 'Diseño Responsive',
                image: 'https://i.imgur.com/s4nkaGt.png',
                text: 'Diseño de paginas web responsive para que tu emprendimiento pueda ser visualizado desde todo dispositivo. En la actualidad una de las partes importantes de un sitio web o aplicación es poder garantizar un correcto desempeño y visualización donde sea que se lo utilice.'
              },
              {
                name: '¿Necesita algo más?',
                image: 'https://i.imgur.com/ACYWGRR.png',
                text: 'Si usted es el tipo de cliente donde día a día se le ocurren nuevas formas de impulsar su negocio o simplemente encuentra antiguo su sitio web actual, puede contactarme para hablar sobre sus ideas o proyectos que tiene en mente para llevar el trabajo en conjunto y mostrarle al mundo esa gran idea suya.'
              }
            ]
          }
        ]
      }
    }
  }
}
</script>
