<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
let ROOT_PATH = 'https://vue-social-cards-sample.netlify.com'
export default {
  name: 'app',
  data() {
    return {
      logo: ROOT_PATH + require('./assets/logo.png')
    }
  },
  components: {
    HelloWorld
  },
  metaInfo() {
    return {
      meta: [
        // Facebook OpenGraph
        {property: 'og:image', content: 'http://dev-api.wya.yoga/mediafiles/school/1/9f8af97f-6e0b-4106-9724-6824a41da02fschool_ex_1_.png'},
        {property: 'og:title', content: 'Facebook Title'},
        {property: 'og:site_name', content: 'Facebook Site Name'},
        {property: 'og:type', content: 'website'},
        {property: 'og:description', content: 'Facebook Description'},
        {property: 'fb:app_id', content: '252804725866373'},
        
        // Twitter Card
        {name: 'twitter:card', content: 'summary'},
        {name: 'twitter:title', content: 'Twitter Title'},
        {name: 'twitter:description', content: 'Twitter Description'},
        {name: 'twitter:image', content: 'http://dev-api.wya.yoga/mediafiles/school/1/9f8af97f-6e0b-4106-9724-6824a41da02fschool_ex_1_.png'},
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
