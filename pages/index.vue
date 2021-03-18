<template>
  <b-container class="px-5 fadeIn bg-dots">
    <b-row>
      <b-col lg="12">
      <!-- <b-img class="w-25 ds" src="~/assets/img/people_working/character 3.svg"></b-img>
      <b-img class="w-25 ds" src="~/assets/img/people_working/character 14.svg"></b-img>
      <b-img class="w-25 ds" src="~/assets/img/people_working/character 16.svg"></b-img> -->
      <b-img class="ds mt-5" style="width: 70vmin; margin-bottom: -34px;" src="~/assets/img/Education/5 SCENE.svg"></b-img>
      <h1 class="display-1 font-weight-bold" v-html="welcome.title"></h1>
      <p class="px-5 mx-5" v-html="welcome.text1"></p>

      <!-- <button v-on:click="isHidden = true">Hide the text below</button>
      <button v-on:click="isHidden = !isHidden">Toggle hide and show</button>
      <h1 v-if="!isHidden">Hide me on click event!</h1> -->

      <div class="links">
        <NuxtLink class="btn btn-lg btn-primary" to="/home">Start your journey!</NuxtLink>       
      </div>
      </b-col>
    </b-row>
    </b-container>
</template>

<script>
import welcome from '../assets/data/welcome.js'

export default {
  transition: {
    name: 'index',
    mode: 'out-in'
  },
  data() {
    return {
      welcome: welcome,
      isHidden: false,
    }
  },
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

    .index-enter-active, 
    .index-leave-active { 
        transition: all 1s ease-in-out;
        }
    .index-enter, 
    .index-leave-active { 
        opacity: 0;
        transform: translateY(-25%); 
        }
</style>