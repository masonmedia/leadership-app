<template>
    <b-container fluid class="bg-dots p-0">
        <b-row class="min-h-100 p-5 rounded ds"> 
            <b-col lg="6" class="d-flex flex-column justify-content-center align-items-start text-left p-5 bg-light rounded-left">
                <svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" fill="currentColor" class="bi bi-cloud-fog2" viewBox="0 0 16 16">
                    <path d="M8.5 4a4.002 4.002 0 0 0-3.8 2.745.5.5 0 1 1-.949-.313 5.002 5.002 0 0 1 9.654.595A3 3 0 0 1 13 13H.5a.5.5 0 0 1 0-1H13a2 2 0 0 0 .001-4h-.026a.5.5 0 0 1-.5-.445A4 4 0 0 0 8.5 4zM0 8.5A.5.5 0 0 1 .5 8h7a.5.5 0 0 1 0 1h-7a.5.5 0 0 1-.5-.5zm0 2a.5.5 0 0 1 .5-.5h9a.5.5 0 0 1 0 1h-9a.5.5 0 0 1-.5-.5z"/>
                </svg>
                <h1 class="fadeIn fw-900" v-html="data.title"></h1>
                <hr class="w-25 mr-auto bg-dark" />
                <!-- <svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" fill="currentColor" class="bi bi-dash" viewBox="0 0 16 16">
                    <path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>
                </svg> -->
                <p class="py-3 mb-0" v-html="data.text1"></p>
                <div class="d-inline my-3">
                    <NuxtLink class="btn btn-lg btn-outline-primary" to="/futureleader" v-html="data.btn1"></NuxtLink>
                    <NuxtLink class="btn btn-lg btn-outline-primary" to="/borntolead" v-html="data.btn2"></NuxtLink> 
                </div>
            </b-col>
            <b-col lg="6" class="d-flex flex-column justify-content-center align-items-center text-center p-0" style="background: pink;">
                <b-img class="fadeIn w-100 h-100 rounded-right ds" style="object-fit: cover" src="~/assets/img/drawkit_economy_finance/REBUILD_THE_ECONOMY.svg"></b-img>
                <!-- <b-img class="fadeIn w-100 h-100 rounded-right shadow" style="object-fit: cover" src="https://picsum.photos/1200/800"></b-img> -->
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
import home from '../assets/data/home.js'

export default {
  transition: {
    name: 'home',
    mode: 'out-in'
  },
  data() {
      return {
          data: home,
      }
  }
  
}
</script>

<style>

    .home-enter-active, 
    .home-leave-active { 
        transition: all 1s ease-in-out; 
        }
    .home-enter, 
    .home-leave-active { 
        opacity: 0;
        /* transition: all 1s ease-in-out; */
        transform: translateY(25%); 
        }
</style>