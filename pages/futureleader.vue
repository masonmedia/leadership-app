<template>
    <b-container fluid class="p-0 bg-dots">
        <b-row class="pt-5 px-5 pb-3 rounded ds">
            <b-col lg="12" class="d-flex flex-column justify-content-center align-items-center text-center bg-light rounded">
                <b-col lg="8" class="p-5">
                    <b-img class="w-50 mx-auto ds" src="~/assets/img/drawkit_economy_finance/9 - ECONOMY ANALYSIS.svg"></b-img>
                    <h1 class="fadeIn fw-900" v-html="data.title"></h1>
                    <hr class="w-25 mx-auto bg-dark" />
                    <p class="py-3 mb-0" v-html="data.text1"></p>
                </b-col>
            </b-col>
        </b-row>
        <b-row class="mx-3">
            <!-- cards -->
            <b-col lg="4" md="6" class="d-flex flex-column justify-content-center align-items-center text-center p-0">
                <div class="p-5 m-3 bg-lightblue rounded">
                    <b-dropdown id="dropdown-right" right no-caret variant="outline" class="m-5" menu-class="text-right bg-lightblue" style="position: absolute; z-index: 1; right: 0; top: 0;">
                            <template v-slot:button-content>
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-three-dots" viewBox="0 0 16 16">
                                    <path d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z"/>
                                </svg>
                            </template>
                        <b-dropdown-item>
                            <div v-b-modal.modal-1>
                                <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" fill="currentColor" class="bi bi-arrows-fullscreen mr-1 mb-1" viewBox="0 0 16 16">
                                    <path fill-rule="evenodd" d="M5.828 10.172a.5.5 0 0 0-.707 0l-4.096 4.096V11.5a.5.5 0 0 0-1 0v3.975a.5.5 0 0 0 .5.5H4.5a.5.5 0 0 0 0-1H1.732l4.096-4.096a.5.5 0 0 0 0-.707zm4.344 0a.5.5 0 0 1 .707 0l4.096 4.096V11.5a.5.5 0 1 1 1 0v3.975a.5.5 0 0 1-.5.5H11.5a.5.5 0 0 1 0-1h2.768l-4.096-4.096a.5.5 0 0 1 0-.707zm0-4.344a.5.5 0 0 0 .707 0l4.096-4.096V4.5a.5.5 0 1 0 1 0V.525a.5.5 0 0 0-.5-.5H11.5a.5.5 0 0 0 0 1h2.768l-4.096 4.096a.5.5 0 0 0 0 .707zm-4.344 0a.5.5 0 0 1-.707 0L1.025 1.732V4.5a.5.5 0 0 1-1 0V.525a.5.5 0 0 1 .5-.5H4.5a.5.5 0 0 1 0 1H1.732l4.096 4.096a.5.5 0 0 1 0 .707z"/>
                                </svg> Quick look
                                <b-modal 
                                ref="modal-1"
                                id="modal-1" 
                                size="xl"
                                centered 
                                title="" 
                                header-class="font-weight-bold pl-5 border-0 rounded-top bg-lightblue"
                                header-close-variant="dark"
                                header-close-content="×"
                                footer-class="bg-lightblue shadow border-0"
                                hide-footer
                                ok-title="Continue"
                                ok-variant="outline-dark"
                                body-class="bg-lightblue">
                                        <b-container fluid class="py-0">
                                            <b-row class="p-3">
                                                <b-col lg="5">
                                                    <b-img class="w-100 ds" src="~/assets/img/drawkit_economy_finance/9 - ECONOMY ANALYSIS.svg"></b-img>
                                                </b-col>
                                                <b-col lg="7" class="d-flex flex-column justify-content-center align-items-start">
                                                    <!-- icon -->
                                                    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" fill="currentColor" class="bi bi-stack" viewBox="0 0 16 16">
                                                        <path d="M14.12 10.163l1.715.858c.22.11.22.424 0 .534L8.267 15.34a.598.598 0 0 1-.534 0L.165 11.555a.299.299 0 0 1 0-.534l1.716-.858 5.317 2.659c.505.252 1.1.252 1.604 0l5.317-2.66zM7.733.063a.598.598 0 0 1 .534 0l7.568 3.784a.3.3 0 0 1 0 .535L8.267 8.165a.598.598 0 0 1-.534 0L.165 4.382a.299.299 0 0 1 0-.535L7.733.063z"/>
                                                        <path d="M14.12 6.576l1.715.858c.22.11.22.424 0 .534l-7.568 3.784a.598.598 0 0 1-.534 0L.165 7.968a.299.299 0 0 1 0-.534l1.716-.858 5.317 2.659c.505.252 1.1.252 1.604 0l5.317-2.659z"/>
                                                    </svg>
                                                    <h6 class="pt-3 pb-2 m-0">Welcome to section 1</h6>
                                                    <h2 class="mt-0">Introduction</h2>
                                                    <!-- dash -->
                                                    <!-- <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" style="margin-left: -12px;" fill="currentColor" class="bi bi-dash float-left mr-auto" viewBox="0 0 16 16">
                                                        <path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>
                                                    </svg> -->
                                                    <hr class="rounded bg-lightcoral border-0 mt-2 mb-3" style="width: 50px; height: 4px;" />
                                                    <p>Irure laborum dolore proident commodo exercitation laborum eiusmod commodo duis sint. Deserunt consequat elit laboris ullamco veniam eiusmod aute aliquip fugiat.</p>
                                                    <div class="d-flex w-100">
                                                        <svg xmlns="http://www.w3.org/2000/svg" width="35" height="35" fill="currentColor" class="bi bi-chevron-double-down mr-2" viewBox="0 0 16 16">
                                                            <path fill-rule="evenodd" d="M1.646 6.646a.5.5 0 0 1 .708 0L8 12.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z"/>
                                                            <path fill-rule="evenodd" d="M1.646 2.646a.5.5 0 0 1 .708 0L8 8.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z"/>
                                                        </svg>
                                                        <!-- <h6 class="font-weight-bold font-italic">Scroll for more info</h6> -->
                                                    </div>
                                                </b-col>
                                                </b-row>
                                                <b-row class="p-3" align-v="baseline">
                                                    <quick-look-item 
                                                    ql-style="bg-img1"
                                                    ql-title="1." 
                                                    ql-text="Identifying customer needs"
                                                    reveal-title="More info"
                                                    reveal-text="Eiusmod ut non sunt laboris consectetur ut. Commodo minim laboris anim consequat dolore eu non. Non Lorem proident occaecat occaecat Lorem sint pariatur non amet dolore. Irure nulla irure amet ipsum duis mollit dolore minim ut reprehenderit nostrud sunt.">
                                                    </quick-look-item>

                                                    <quick-look-item 
                                                    ql-style="bg-img2"
                                                    ql-title="2." 
                                                    ql-text="Building better relationships with customers"
                                                    reveal-title="More info"
                                                    reveal-text="Ipsum commodo ipsum adipisicing Lorem ullamco cupidatat officia cillum Lorem consequat culpa labore incididunt. In anim ullamco id voluptate id enim commodo pariatur proident. Nisi elit proident velit mollit dolore qui occaecat veniam. Exercitation ad pariatur sit laborum consectetur deserunt laboris dolor id. Et id officia voluptate exercitation.">
                                                    </quick-look-item>
                                                    
                                                    <quick-look-item 
                                                    ql-style="bg-img3"
                                                    ql-title="3." 
                                                    ql-text="Dealing with negative customer feedback"
                                                    reveal-title="More info"
                                                    reveal-text="Lorem cillum ullamco laborum elit labore nisi duis dolor commodo enim sint. Nulla labore tempor velit pariatur laboris cillum fugiat. Pariatur nulla labore magna incididunt fugiat esse pariatur id minim ea voluptate do. Ipsum ea minim aliqua velit esse. Ea pariatur amet id amet reprehenderit laborum. Occaecat qui labore qui occaecat ipsum officia tempor velit consectetur incididunt ad pariatur incididunt.">
                                                    </quick-look-item>
                                                    
                                                    <quick-look-item
                                                    ql-style="bg-img4" 
                                                    ql-title="4." 
                                                    ql-text="Building better relationships with customers and colleagues"
                                                    reveal-title="More info"
                                                    reveal-text="Lorem in culpa esse dolore voluptate laboris ut id amet magna labore nulla consectetur dolore. Sunt eu dolor ullamco cillum in ut dolore non consectetur. Amet sunt proident tempor sint laborum tempor duis duis ut exercitation cupidatat dolor. Et dolor pariatur cillum ea pariatur cupidatat nisi cillum ut labore. Occaecat duis qui veniam fugiat quis.">
                                                    </quick-look-item>
                                                    
                                                    <quick-look-item 
                                                    ql-style="bg-img5"
                                                    ql-title="5." 
                                                    ql-text="Being more focused; mindful"
                                                    reveal-title="More info"
                                                    reveal-text="Consequat cupidatat voluptate officia ex ullamco. Tempor in ex minim sit est ullamco. Aute Lorem id nostrud proident proident occaecat laborum sint incididunt. Amet pariatur non culpa sunt pariatur velit Lorem deserunt. Tempor labore nisi officia irure pariatur.">
                                                    </quick-look-item>
                                                <!-- footer buttons -->
                                                <b-col lg="12" class="d-flex justify-content-end align-items-center pt-4 pb-3 pr-4 mt-3">
                                                    <b-button class="mr-2" variant="outline-dark" @click="hideModal">Close</b-button>
                                                    <b-button variant="coral">
                                                        <NuxtLink class="text-light" to="/one">Learn more</NuxtLink>
                                                    </b-button>
                                                </b-col>
                                            </b-row>
                                        </b-container>
                                </b-modal>
                            </div>
                        </b-dropdown-item>
                        <NuxtLink class="dropdown-item" to="/one">
                            <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" fill="currentColor" class="bi bi-box-arrow-up-right mr-1 mb-1" viewBox="0 0 16 16">
                                <path fill-rule="evenodd" d="M8.636 3.5a.5.5 0 0 0-.5-.5H1.5A1.5 1.5 0 0 0 0 4.5v10A1.5 1.5 0 0 0 1.5 16h10a1.5 1.5 0 0 0 1.5-1.5V7.864a.5.5 0 0 0-1 0V14.5a.5.5 0 0 1-.5.5h-10a.5.5 0 0 1-.5-.5v-10a.5.5 0 0 1 .5-.5h6.636a.5.5 0 0 0 .5-.5z"/>
                                <path fill-rule="evenodd" d="M16 .5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793L6.146 9.146a.5.5 0 1 0 .708.708L15 1.707V5.5a.5.5 0 0 0 1 0v-5z"/>
                            </svg> Deep dive
                        </NuxtLink>
                    </b-dropdown>
                    <b-img class="fadeIn ds" style="width: 200px; height: 200px" src="~/assets/img/drawkit_economy_finance/REBUILD_THE_ECONOMY.svg"></b-img>
                    <h3>Leadership 1</h3>
                    <p>Do veniam dolore consectetur pariatur elit velit ad dolor incididunt sint dolor incididunt nostrud.</p>
                    <!-- <div class="d-inline">
                        <b-button v-b-modal.modal-2>Quick look</b-button>
                        <b-modal id="modal-2" size="xl" centered title="BootstrapVue">
                            <p class="my-4">Vertically centered modal!</p>
                        </b-modal>
                        <b-button variant="outline-dark">Deep dive</b-button>
                    </div> -->
                </div>
            </b-col>
            <b-col lg="4" md="6" class="d-flex flex-column justify-content-center align-items-center text-center p-0">
                <div class="p-5 m-3 bg-salmon rounded-lg">
                    <b-dropdown id="dropdown-right" right no-caret variant="outline" class="m-5" menu-class="text-right bg-salmon" style="position: absolute; z-index: 1; right: 0; top: 0;">
                            <template v-slot:button-content>
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-three-dots" viewBox="0 0 16 16">
                                    <path d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z"/>
                                </svg>
                            </template>
                        <b-dropdown-item>
                            <div v-b-modal.modal-2>Quick look
                                <b-modal 
                                id="modal-2" 
                                size="xl" 
                                centered 
                                title="" 
                                header-class="font-weight-bold pl-5 border-0 rounded-top bg-salmon"
                                header-close-variant="dark"
                                header-close-content="×"
                                footer-class="bg-salmon shadow border-0"
                                hide-footer
                                ok-only
                                ok-title="Continue"
                                ok-variant="light"
                                body-class="bg-salmon">
                                        <b-container fluid class="py-0">
                                            <b-row class="p-3">
                                                <b-col lg="5">
                                                    <b-img class="w-100 ds" src="~/assets/img/drawkit_economy_finance/9 - ECONOMY ANALYSIS.svg"></b-img>
                                                </b-col>
                                                <b-col lg="7" class="d-flex flex-column justify-content-center align-items-start">
                                                    <!-- icon -->
                                                    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" fill="currentColor" class="bi bi-stack" viewBox="0 0 16 16">
                                                        <path d="M14.12 10.163l1.715.858c.22.11.22.424 0 .534L8.267 15.34a.598.598 0 0 1-.534 0L.165 11.555a.299.299 0 0 1 0-.534l1.716-.858 5.317 2.659c.505.252 1.1.252 1.604 0l5.317-2.66zM7.733.063a.598.598 0 0 1 .534 0l7.568 3.784a.3.3 0 0 1 0 .535L8.267 8.165a.598.598 0 0 1-.534 0L.165 4.382a.299.299 0 0 1 0-.535L7.733.063z"/>
                                                        <path d="M14.12 6.576l1.715.858c.22.11.22.424 0 .534l-7.568 3.784a.598.598 0 0 1-.534 0L.165 7.968a.299.299 0 0 1 0-.534l1.716-.858 5.317 2.659c.505.252 1.1.252 1.604 0l5.317-2.659z"/>
                                                    </svg>
                                                    <h6 class="pt-3 pb-2 m-0">Welcome to section 2</h6>
                                                    <h2 class="mb-0 mt-0">Introduction</h2>
                                                    <!-- dash -->
                                                    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" style="margin-left: -12px;" fill="currentColor" class="bi bi-dash float-left mr-auto" viewBox="0 0 16 16">
                                                        <path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>
                                                    </svg>
                                                    <p>Irure laborum dolore proident commodo exercitation laborum eiusmod commodo duis sint. Deserunt consequat elit laboris ullamco veniam eiusmod aute aliquip fugiat.</p>
                                                </b-col>
                                                </b-row>
                                                <b-row class="p-3">
                                                <b-col xl="3" lg="6" class="">
                                                    <div class="p-5 m-2 bg-glass rounded-xl shadow">
                                                        <h3>Topic 1</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-glass rounded-xl shadow">
                                                        <h3>Topic 2</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-glass rounded-xl shadow">
                                                        <h3>Topic 3</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-glass rounded-xl shadow">
                                                        <h3>Topic 4</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <!-- footer buttons -->
                                                <b-col lg="12" class="d-flex justify-content-end align-items-center pt-4 pb-3 pr-4 mt-3">
                                                    <b-button class="mr-2" variant="outline-dark" @click="hideModal">Close</b-button>
                                                    <b-button variant="info">
                                                        <NuxtLink class="text-light" to="/one">Learn more</NuxtLink>
                                                    </b-button>
                                                </b-col>
                                            </b-row>
                                        </b-container>
                                </b-modal>
                            </div>
                        </b-dropdown-item>
                        <NuxtLink class="dropdown-item" to="/">Deep dive</NuxtLink>
                    </b-dropdown>
                    <b-img class="fadeIn ds" style="width: 200px; height: 200px" src="~/assets/img/drawkit_economy_finance/9 - ECONOMY ANALYSIS.svg"></b-img>
                    <h3>Leadership 2</h3>
                    <p>Do veniam dolore consectetur pariatur elit velit ad dolor incididunt sint dolor incididunt nostrud.</p>
                </div>
            </b-col>
            <b-col lg="4" md="6" class="d-flex flex-column justify-content-center align-items-center text-center p-0">
                <div class="p-5 m-3 bg-lightgoldenrod rounded-lg">
                    <b-dropdown id="dropdown-right" right no-caret variant="outline" class="m-5" menu-class="text-right bg-lightgoldenrod" style="position: absolute; z-index: 1; right: 0; top: 0;">
                            <template v-slot:button-content>
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-three-dots" viewBox="0 0 16 16">
                                    <path d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z"/>
                                </svg>
                            </template>
                        <b-dropdown-item>
                            <div v-b-modal.modal-3>Quick look
                                <b-modal 
                                id="modal-3" 
                                size="xl" 
                                centered 
                                title="" 
                                header-class="font-weight-bold pl-5 border-0 rounded-top bg-lightgoldenrod"
                                header-close-variant="dark"
                                header-close-content="×"
                                footer-class="bg-lightgoldenrod shadow border-0"
                                ok-only
                                ok-title="Continue"
                                ok-variant="outline-dark"
                                body-class="bg-lightgoldenrod">
                                        <b-container fluid class="py-0">
                                            <b-row class="p-3">
                                                <b-col lg="5">
                                                    <b-img class="w-100 ds" src="~/assets/img/drawkit_economy_finance/9 - ECONOMY ANALYSIS.svg"></b-img>
                                                </b-col>
                                                <b-col lg="7" class="d-flex flex-column justify-content-center align-items-start">
                                                    <!-- icon -->
                                                    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" fill="currentColor" class="bi bi-stack" viewBox="0 0 16 16">
                                                        <path d="M14.12 10.163l1.715.858c.22.11.22.424 0 .534L8.267 15.34a.598.598 0 0 1-.534 0L.165 11.555a.299.299 0 0 1 0-.534l1.716-.858 5.317 2.659c.505.252 1.1.252 1.604 0l5.317-2.66zM7.733.063a.598.598 0 0 1 .534 0l7.568 3.784a.3.3 0 0 1 0 .535L8.267 8.165a.598.598 0 0 1-.534 0L.165 4.382a.299.299 0 0 1 0-.535L7.733.063z"/>
                                                        <path d="M14.12 6.576l1.715.858c.22.11.22.424 0 .534l-7.568 3.784a.598.598 0 0 1-.534 0L.165 7.968a.299.299 0 0 1 0-.534l1.716-.858 5.317 2.659c.505.252 1.1.252 1.604 0l5.317-2.659z"/>
                                                    </svg>
                                                    <h6 class="pt-3 pb-2 m-0">Welcome to section 3</h6>
                                                    <h2 class="mb-0 mt-0">Introduction</h2>
                                                    <!-- dash -->
                                                    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" style="margin-left: -12px;" fill="currentColor" class="bi bi-dash float-left mr-auto" viewBox="0 0 16 16">
                                                        <path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>
                                                    </svg>
                                                    <p>Irure laborum dolore proident commodo exercitation laborum eiusmod commodo duis sint. Deserunt consequat elit laboris ullamco veniam eiusmod aute aliquip fugiat.</p>
                                                </b-col>
                                                </b-row>
                                                <b-row class="p-3">

                                                <b-col xl="3" lg="6" class="">
                                                    <div class="p-5 m-2 bg-glass rounded-xl shadow">
                                                        <h3>Topic 1</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-glass rounded-xl shadow">
                                                        <h3>Topic 2</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-glass rounded-xl shadow">
                                                        <h3>Topic 3</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-glass rounded-xl shadow">
                                                        <h3>Topic 4</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                            </b-row>
                                        </b-container>
                                </b-modal>
                            </div>
                        </b-dropdown-item>
                        <NuxtLink class="dropdown-item" to="/">Deep dive</NuxtLink>
                    </b-dropdown>
                    <b-img class="fadeIn ds" style="width: 200px; height: 200px" src="~/assets/img/drawkit_economy_finance/3 - JOB LOOKING.svg"></b-img>
                    <h3>Leadership 3</h3>
                    <p>Do veniam dolore consectetur pariatur elit velit ad dolor incididunt sint dolor incididunt nostrud.</p>
                </div>
            </b-col>

            <!-- row 2 -->
            <b-col lg="4" md="6" class="d-flex flex-column justify-content-center align-items-center text-center p-0">
                <div class="p-5 m-3 bg-lightcoral rounded">
                    <b-dropdown id="dropdown-right" right no-caret variant="outline" class="m-5" menu-class="text-right bg-lightcoral" style="position: absolute; z-index: 1; right: 0; top: 0;">
                            <template v-slot:button-content>
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-three-dots" viewBox="0 0 16 16">
                                    <path d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z"/>
                                </svg>
                            </template>
                        <b-dropdown-item>
                            <div v-b-modal.modal-4> Quick look
                                <b-modal 
                                id="modal-4" 
                                size="xl" 
                                centered 
                                title="Future One" 
                                header-class="border-0"
                                ok-only
                                ok-title="Continue"
                                ok-variant="outline-dark">
                                    <p class="my-4">
                                        <b-container fluid>
                                            <b-row>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-warning ds rounded-lg">
                                                        <h3>Topic 1</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-warning ds rounded-lg">
                                                        <h3>Topic 1</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-warning ds rounded-lg">
                                                        <h3>Topic 1</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                                <b-col xl="3" lg="6">
                                                    <div class="p-5 m-2 bg-warning ds rounded-lg">
                                                        <h3>Topic 1</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                            </b-row>
                                        </b-container>
                                    </p>
                                </b-modal>
                            </div>
                        </b-dropdown-item>
                        <NuxtLink class="dropdown-item" to="/">Deep dive</NuxtLink>
                    </b-dropdown>
                    <b-img class="fadeIn ds" style="width: 200px; height: 200px" src="~/assets/img/drawkit_economy_finance/REBUILD_THE_ECONOMY.svg"></b-img>
                    <h3>Leadership</h3>
                    <p>Do veniam dolore consectetur pariatur elit velit ad dolor incididunt sint dolor incididunt nostrud.</p>
                </div>
            </b-col>
            <b-col lg="4" md="6" class="d-flex flex-column justify-content-center align-items-center text-center p-0">
                <div class="p-5 m-3 bg-lightskyblue rounded-lg">
                    <b-dropdown id="dropdown-right" right no-caret variant="outline" class="m-5" menu-class="text-right bg-lightskyblue" style="position: absolute; z-index: 1; right: 0; top: 0;">
                            <template v-slot:button-content>
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-three-dots" viewBox="0 0 16 16">
                                    <path d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z"/>
                                </svg>
                            </template>
                        <b-dropdown-item>
                            <div v-b-modal.modal-5>Quick look
                                <b-modal 
                                id="modal-5" 
                                size="xl" 
                                centered 
                                title="Future Two" 
                                header-class="border-0"
                                ok-only
                                ok-title="Continue"
                                ok-variant="outline-dark">
                                    <p class="my-4">
                                        <b-container fluid>
                                            <b-row>
                                                <b-col lg="3">
                                                    <div class="p-5 m-3 bg-warning ds rounded-lg">
                                                        <h3>Topic 1</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                            </b-row>
                                        </b-container>
                                    </p>
                                </b-modal>
                            </div>
                        </b-dropdown-item>
                        <NuxtLink class="dropdown-item" to="/">Deep dive</NuxtLink>
                    </b-dropdown>
                    <b-img class="fadeIn ds" style="width: 200px; height: 200px" src="~/assets/img/drawkit_economy_finance/9 - ECONOMY ANALYSIS.svg"></b-img>
                    <h3>Leadership</h3>
                    <p>Do veniam dolore consectetur pariatur elit velit ad dolor incididunt sint dolor incididunt nostrud.</p>
                </div>
            </b-col>
            <b-col lg="4" md="6" class="d-flex flex-column justify-content-center align-items-center text-center p-0">
                <div class="p-5 m-3 bg-lightcyan rounded-lg">
                    <b-dropdown id="dropdown-right" right no-caret variant="outline" class="m-5" menu-class="text-right bg-lightcyan" style="position: absolute; z-index: 1; right: 0; top: 0;">
                            <template v-slot:button-content>
                                <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-three-dots" viewBox="0 0 16 16">
                                    <path d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z"/>
                                </svg>
                            </template>
                        <b-dropdown-item>
                            <div v-b-modal.modal-6>Quick look
                                <b-modal 
                                id="modal-6" 
                                size="xl" 
                                centered 
                                title="Future Three" 
                                header-class="border-0"
                                ok-only
                                ok-title="Continue"
                                ok-variant="outline-dark">
                                    <p class="my-4">
                                        <b-container fluid>
                                            <b-row>
                                                <b-col lg="3">
                                                    <div class="p-5 m-3 bg-warning ds rounded-lg">
                                                        <h3>Topic 1</h3>
                                                        <p>More info here lorem lorem lorem</p>   
                                                    </div>
                                                </b-col>
                                            </b-row>
                                        </b-container>
                                    </p>
                                </b-modal>
                            </div>
                        </b-dropdown-item>
                        <NuxtLink class="dropdown-item" to="/">Deep dive</NuxtLink>
                    </b-dropdown>
                    <b-img class="fadeIn ds" style="width: 200px; height: 200px" src="~/assets/img/drawkit_economy_finance/3 - JOB LOOKING.svg"></b-img>
                    <h3>Leadership</h3>
                    <p>Do veniam dolore consectetur pariatur elit velit ad dolor incididunt sint dolor incididunt nostrud.</p>
                </div>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
import future from '../assets/data/futureleader.js'
import QuickLookItem from '../components/QuickLookItem.vue'

export default {
    scrollToTop: false,
    transition: {
        name: 'future',
        mode: 'out-in'
    },
    components: {
        QuickLookItem,
    },
    data() {
        return {
            data: future,
            isHidden: true,
            detailsAreVisible: false,
        }
    },
    methods: {
        hideModal() {
            this.$refs['modal-1'].hide()
        },
        toggleDetails() {
            //   set detailsAreVisible to what they currently are NOT
            this.detailsAreVisible = !this.detailsAreVisible;
        },
    }
}
</script>

<style>

    .future-enter-active, 
    .future-leave-active { 
        transition: all 1s ease-in-out; 
        }
    .future-enter, 
    .future-leave-active { 
        opacity: 0;
        /* transition: all 1s ease-in-out; */
        transform: translateY(-25%) scale(0.9); 
        }
</style>