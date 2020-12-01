<template>
  <div id="app">
   <div class="home">
    <place-holder/>
    </div>
    <div id="footer" class="mt-2">
      <div class="social-icons-wrapper">
       
        <a href="https://twitter.com/VuejsNg" target="_blank" title="Our Twitter">
          <fa :icon="['fab', 'twitter-square']" class="social__icon"/>
        </a>
        <a href="https://www.meetup.com/vuejs-nigeria/" target="_blank" title="Our Meetup group">
          <fa :icon="['fab', 'meetup']" class="social__icon"/>
        </a>

        <a href="https://www.youtube.com/channel/UCjswIt8G9_zlAnNo47u98BQ" target="_blank" title="Our Youtube">
          <fa :icon="['fab', 'youtube-square']" class="social__icon"/>
        </a>

         <a href="https://medium.com/@vuejsnigeria" target="_blank" title="Our Medium">
          <fa :icon="['fab', 'medium']" class="social__icon"/>
        </a>

        <a href="https://dev.to/vuejsng" target="_blank" title="Our Dev.to">
          <fa :icon="['fab', 'dev']" class="social__icon"/>
        </a>
      </div>
    </div>
    <div class="credits">
    Thanks to  <a href="https://mayashavin.com/" title="Maya Shavin">Maya</a> and <a href="https://www.dimshik.com/" title="Dima Vishnevetsky">Dima</a> who built the original site for  <a href="https://www.vuejsisrael.com/" title="vuejs israel"> Vue.js Israel </a> ♥
    </div>
  </div>
</template>

<script>
import PlaceHolder from '~/components/PlaceHolder.vue'

export default {
  components: {
    PlaceHolder
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
}
#nav {
  padding: 30px;
}
#nav a {
  font-weight: bold;
  color: #2c3e50;
}
#nav a.router-link-exact-active {
  color: #42b983;
}
#footer {
  font-size: 35px;
  display: flex;
  justify-content: center;
}
.social__icon {
  margin: 5px;
  color: #263e51;
}
.social-icons-wrapper{
  max-width: 500px;
  width: 100%;
  min-width: 300px;
  display: flex;
  justify-content: space-around;
}
.credits {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0px;
  padding-bottom: 0.5rem;
  color: #263e51;
}
.credits a,
.credits a:active {
  color: #263e51;
}
</style>
