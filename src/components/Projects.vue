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
      <div class="projects__info" v-html="cards.info[0].title">
        <p>
          <strong>{{title}}</strong>
        </p>
      </div>
      <br>
      <!-- <div class="projects__works">
        <div class="card" v-for="(item, index) in cards.info[0].variants" :key="index">
          <img :src="item.image" alt="project">
          <div class="card--active">
            {{item.name}} <br>
            {{item.text}}
          </div>
        </div>
      </div> -->
      <section class="card-list" >
        <article class="card" v-for="(item, index) in cards.info[0].variants" :key="index">
          <header class="card-header">
            <h2>{{item.name}}</h2>
          </header>

          <div>
            <img :src="item.image" alt="project">
          </div>

            <div class="author-name">
              <p>{{item.text}}</p>
              <a href="https://github.com/JuanLoyola" target="_blank">Github</a> (EN PROCESO)
            </div>
          <div class="tags">
            <p>html</p>
            <p>css</p>
            <p>vue.js</p>
          </div>
        </article>
      </section>
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

      .card-list {
      display: flex;
      padding: 3rem;
      overflow-x: scroll;
    }

      .card-list::-webkit-scrollbar {
        width: 10px;
        height: 10px;
      }

      .card-list::-webkit-scrollbar-track {
        background: #fff;
      }

      .card {
        height: 350px;
        width: 200px;
        min-width: 250px;
        padding: 1.5rem;
        border-radius: 16px;
        background: #17141d;
        box-shadow: -1rem 0 1rem #000;
        display: flex;
        flex-direction: column;
        transition: .2s;
        margin: 0;
        scroll-snap-align: start;
        clear: both;
        position: relative;
      }

      .card img{
        width: 100%;
      }

      .card:focus-within~.card, .card:hover~.card {
        transform: translateX(130px);
      }

      .card:hover {
        transform: translateY(-1rem);
      }

      .card:not(:first-child) {
        margin-left: -130px;
      }

      .card-header {
        margin-bottom: auto;
      }

      .card-header h2 {
        font-size: 20px;
        margin: .25rem 0 auto;
        text-decoration: none;
        color: #fff;
        border: 0;
        display: inline-block;
        cursor: pointer;
      }

      .card-author {
        margin: 3rem 0 0;
        display: grid;
        grid-template-columns: 75px 1fr;
        align-items: center;
        position: relative;
      }

      .author-name {
        grid-area: auto;
        box-sizing: border-box;
        color: #6d6a6a;
      }

      .author-name p{
        grid-area: auto;
        box-sizing: border-box;
        color: #f1f1f1;
        font-size: 13px;
        text-align: start;
      }

      .author-name a{
        color: rgb(194, 146, 238);
      }

      .tags {
        margin: 1rem 0 2rem;
        padding: .5rem 0 1rem;
        line-height: 2;
        margin-bottom: 0;
        display:flex;
        flex-direction: row;
      }

      .tags p {
        font-style: normal;
        font-weight: 70px;
        width: 15%;
        font-size: .5rem;
        color: #7a7a8c;
        text-transform: uppercase;
        display:flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        font-size: .66rem;
        border: 3px solid #28242f;
        border-radius: 2rem;
        padding: .2rem .2rem .2rem;
      }

      .tags p:hover {
        border: 3px solid rgb(146, 142, 142);
        box-shadow: rgb(145, 141, 141) 1px 0px 28px;
        color: #f1f1f1;
        cursor:pointer;
      }
    }
  }
</style>

<script>
export default {
  name: 'Projects',
  data () {
    return {
      cards: {
        info: [
          {
            title: 'Creo proyectos fuertes, con identidad.',
            variants: [
              {
                name: 'Birds',
                image: 'https://i.imgur.com/gB9SkK8.png',
                text: 'Diseño y desarrollo de landing page, proyecto usando REST API.'
              },
              {
                name: 'Tanzee Co',
                image: 'https://i.imgur.com/Xhs9gXO.png',
                text: 'Diseño y desarrollo de landing page para una startup.'
              },
              {
                name: 'Parallax',
                image: 'https://i.imgur.com/4UGWcqj.png',
                text: 'Diseño y desarrollo de landing page con efecto parallax y animaciones, proyecto a modo de práctica.'
              },
              {
                name: 'Vr film',
                image: 'https://i.imgur.com/LSDOHmK.png',
                text: 'Diseño y desarrollo de landing page para una pelicula realizada en realidad virtual.'
              },
              {
                name: 'Yoga APP',
                image: 'https://i.imgur.com/ivUnXYm.png',
                text: 'Diseño y desarrollo de landing page para aplicacion de Yoga, proyecto personal usando REST API. '
              },
              {
                name: 'Landing for e-commerce',
                image: 'https://i.imgur.com/H4VNBDP.png',
                text: 'Diseño y desarrollo de landing page para E-commerce.'
              }
            ]
          }
        ]
      }
    }
  }
}
</script>
