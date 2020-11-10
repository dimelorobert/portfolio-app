<template>
  <div class="container">
    <div id="portfolio" class="banner">
      <div class="banner__info">
        <h2>
          {{$t('project.banner')}}
        </h2>
        <a href="#contact">
          {{$t('project.btn')}}
        </a>
      </div>
    </div>
    <div class="projects">
      <div class="projects__info">
        <p>
          <strong>{{$t('project.text')}}</strong>
        </p>
      </div>
      <br>
      <section class="card-list" >
        <article class="card" v-for="(item, index) in cards.info[0].variants" :key="index">
          <header class="card-header">
            <h2>{{item.name}}</h2>
          </header>

          <div>
            <img :src="item.image" alt="project">
          </div>

            <div class="author-name">
              <a :href= "item.github" target="_blank">Github</a>
              <a :href= "item.live" target="_blank" >Live</a>
            </div>
          <div class="tags">
            <p>{{item.html}}</p>
            <p>{{item.css}}</p>
            <p>{{item.javascript  || item.vue}}</p>
          </div>
        </article>
      </section>
      <p class="alert"> {{$t('project.alert')}}</p>
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
        margin: 20px;
        width: auto;
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
        box-shadow: -1rem 0 1rem rgba(0, 0, 0, 0.644);
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
        margin-bottom: 50px;
      }

      .card-header h2 {
        font-size: 20px;
        margin: .30rem 0 auto;
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

      .author-name a{
        color: rgb(194, 146, 238);
        display:flex;
        font-weight: 600;
        justify-content: flex-start;
        margin: 10px 2px;
      }

      .tags {
        margin: 0.5rem 0 2rem;
        margin-bottom: 0;
        display:flex;
        flex-direction: row;
        align-items: flex-start;
        justify-content: flex-start;
      }

      .tags p {
        font-style: normal;
        font-weight: 70px;
        width: 25%;
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
        border: 3px solid rgba(60, 220, 231, 0.726);
        box-shadow: rgb(88, 180, 241) 1px 0px 28px;
        color: #f1f1f1;
        cursor:pointer;
      }
    }
  }

@media screen and (min-width:320px) and (max-width: 320px){
  .container{

    .banner{

      &__info h2{
        font-size: 15px;
      }

      &__info a{
        font-size: 13px;
      }
    }
    overflow: hidden;
  }

  .projects{
    width: 100%;
    &__info{
      width: 55px;
      font-size:0.9rem;
      font-weight: bold;
      text-align: center;
      border-top: 5px solid #1DAEEC; /* seguir aca */
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
            variants: [
              {
                name: '3D Mario Bros Card',
                image: 'https://i.imgur.com/PTXzEFS.png',
                github: 'https://github.com/JuanLoyola/mario',
                live: 'https://mymario.netlify.app',
                html: 'html',
                css: 'css',
                javascript: 'javascript'
              },
              {
                name: 'Blog',
                image: 'https://i.imgur.com/ooBz5sf.png',
                github: 'https://github.com/JuanLoyola/Blog-Animations',
                live: 'https://blog-animations.hostman.site',
                html: 'html',
                css: 'css',
                vue: 'vue.js'
              },
              {
                name: 'Generate Password',
                image: 'https://i.imgur.com/oedfnL8.png',
                github: 'https://github.com/JuanLoyola/generatePassword',
                live: 'https://genthepass.netlify.app',
                html: 'html',
                css: 'css',
                javascript: 'javascript'
              },
              {
                name: ' Nails',
                image: 'https://i.imgur.com/QIq0W3E.png',
                github: 'https://github.com/JuanLoyola/Nails-lading',
                live: 'https://lorem-nails.netlify.app',
                html: 'html',
                css: 'css',
                vue: 'vue.js'
              },
              {
                name: 'Pumita Shoes',
                image: 'https://i.imgur.com/QQ2D76s.png',
                html: 'html',
                css: 'css',
                vue: 'vue.js'
              },
              {
                name: 'Punchbag minigame',
                image: 'https://i.imgur.com/v6pBR0M.png',
                github: 'https://github.com/JuanLoyola/punchbag-game',
                live: 'https://punchbag-game.netlify.app',
                html: 'html',
                css: 'css',
                vue: 'vue.js'
              },
              {
                name: 'Weather app',
                image: 'https://i.imgur.com/Bxy6Oy0.png',
                github: 'https://github.com/JuanLoyola/weather-app',
                live: 'https://weather-app-afa7.hostman.site',
                html: 'html',
                css: 'css',
                vue: 'vue.js'
              }
            ]
          }
        ]
      }
    }
  }
}
</script>
