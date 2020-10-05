<template>
  <div class="container">
    <div class="container__info">
      <p>
        © Hecho con &lt;3 por <strong>Juan Loyola</strong>. HTML, CSS, JS  (w/ Vue.js) | Hosted by Hostman
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .container{
    width: 100%;
    height: 8vh;
    background: rgba(51, 51, 51, 0.884);
    margin: 0px;
    display:flex;
    justify-content: flex-end;
    align-items: center;
    &__info{
      font-family: 'Poppins';
      font-size: 16px;
      line-height: 24px;
      display: flex;
      color: #f1f1f1;
    }
    &__info strong{
      color: rgb(248, 134, 93);
    }
  }
</style>
<script>
export default {
  name: 'Footer'
}
</script>
