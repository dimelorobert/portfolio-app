<template>
  <div class="locale-changer">
    <div >
      <select class="language" v-model="$i18n.locale">
        <option v-for="(lang, i) in langs" :key="`Lang${i}`" :value="lang">{{ lang }}</option>
      </select>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.language{
  width: 50px;
  height: 30px;
  color: #f1f1f1;
  background: #333;
  border: 1px solid white;
  margin: 0 20px;
  font-weight: bold;
  font-family: 'Poppins';
}
</style>

<script>
export default {
  name: 'languageSwitcher',
  data () {
    return {
      langs: [
        'es', 'en'
      ]
    }
  }
}
</script>
