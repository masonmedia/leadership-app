<template>
    <b-container fluid class="bg-dots p-0">
        <b-row class="min-h-100 p-5 rounded ds">
            <b-col lg="6" class="d-flex flex-column justify-content-center align-items-start text-left p-5 bg-lightgoldenrod rounded-left">
                <b-img class="fadeIn rounded ds" style="width: 200px; height: 200px;" src="~/assets/img/drawkit_economy_finance/REBUILD_THE_ECONOMY.svg"></b-img>
                <!-- <svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" fill="currentColor" class="bi bi-columns mb-3" viewBox="0 0 16 16">
                    <path d="M0 2a1 1 0 0 1 1-1h14a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V2zm8.5 0v8H15V2H8.5zm0 9v3H15v-3H8.5zm-1-9H1v3h6.5V2zM1 14h6.5V6H1v8z"/>
                </svg> -->
                <h1 class="fadeIn fw-900">Leadership 1</h1>
                <hr class="rounded bg-lightcoral border-0 mt-2 mb-3" style="width: 50px; height: 4px;" />
                <p class="py-3 mb-0">Esse consectetur ex consectetur cillum magna occaecat pariatur laboris voluptate ad. Consequat est mollit amet do culpa cillum elit dolore. Enim nostrud nisi et velit mollit. Sint consectetur amet nisi aliquip ipsum minim ut esse velit nostrud veniam excepteur adipisicing ad. Anim eu elit fugiat do quis excepteur sint eu eu.</p>
                <b-button variant="coral">Read more</b-button>
            </b-col>
            <b-col lg="6" class="d-flex flex-column justify-content-center align-items-center text-center p-0" style="background: pink;">
                <iframe width="100%" height="100%" src="https://www.youtube.com/embed/XGQo-Vge-WU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
    name: 'one',
    transition: {
        name: 'home',
    }
}
</script>