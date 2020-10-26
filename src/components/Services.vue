<template>
  <div id="service" class="container">
    <div class="container__card" v-for="(item, index) in images.variant" :key="index">
      <div class="card__title">
        <h2>
          {{$t('services[0].title')}}
        </h2>
        <img :src="item.image" alt="projects">
      </div>
      <p>{{$t('services[1].content')}}</p>
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
      images: {
        variant: [
          {
            image: 'https://i.imgur.com/yZevfRF.png'
          },
          {
            image: 'https://i.imgur.com/M0UoXXG.png'
          },
          {
            image: 'https://i.imgur.com/s4nkaGt.png'
          },
          {
            image: 'https://i.imgur.com/ACYWGRR.png'
          }
        ]
      }
    }
  }
}
</script>
