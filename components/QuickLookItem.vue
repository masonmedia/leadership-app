<template>
    <b-col xl="12">
        <div class="p-5 m-2 bg-glass rounded-xl shadow" style="position: relative;">
            <b-row class="d-flex justify-content-start align-items-center">
                <b-col xl="5" lg="12" class="d-flex flex-column justify-content-end align-items-start">
                    <h3 class="display-3 text-lightcoral font-weight-bold">#{{ qlTitle }}</h3>
                    <p class="h4 text-muted">{{ qlText }}</p>  
                    <!-- <b-button variant="outline-dark" class="" v-on:click="isHidden = false">Read more</b-button> -->
                    <b-button variant="coral" class="mt-2" @click="toggleDetails">Read more</b-button>
                </b-col>
                <!-- show more -->
                <transition name="index">
                    <b-col xl="7" lg="12" class="fadeIn d-flex flex-column justify-content-end align-items-start" v-if="detailsAreVisible">
                        <h3>{{ revealTitle }} <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" fill="lightcoral" class="bi bi-check2-all" viewBox="0 0 16 16">
                            <path d="M12.354 4.354a.5.5 0 0 0-.708-.708L5 10.293 1.854 7.146a.5.5 0 1 0-.708.708l3.5 3.5a.5.5 0 0 0 .708 0l7-7zm-4.208 7l-.896-.897.707-.707.543.543 6.646-6.647a.5.5 0 0 1 .708.708l-7 7a.5.5 0 0 1-.708 0z"/>
                            <path d="M5.354 7.146l.896.897-.707.707-.897-.896a.5.5 0 1 1 .708-.708z"/>
                            </svg>
                            <!-- <NuxtLink to="/one"> <b-button class="btn" variant="outline-coral">more</b-button></NuxtLink> -->
                        </h3>
                        <hr class="rounded bg-lightcoral border-0 mt-2 mb-3" style="width: 50px; height: 4px;" />
                        <p class="mb-0">{{ revealText }}</p>
                    </b-col>
                    <transition name="index" v-else>
                    <b-col xl="7" lg="12" :class="qlStyle" class="w-100 h-100 d-flex flex-column justify-content-end align-items-center p-0" style="position: absolute; right: 0;">
                    </b-col> 
                    </transition>
                </transition>

            </b-row>
        </div>
    </b-col>
</template>

<script>
export default {
    name: 'quick-look',
    props: [
        'qlTitle',
        'qlText',
        'revealTitle',
        'revealText',
        'imgUrl',
        'qlStyle',
    ],
    data() {
        return {
            detailsAreVisible: false,
        }
    },
    methods: {
        toggleDetails() {
        //   set detailsAreVisible to what they currently are NOT
          this.detailsAreVisible = !this.detailsAreVisible;
      },
    }
}
</script>