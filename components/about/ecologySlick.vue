<template>
    <VueSlickCarousel v-bind="settings" class="ecology__slick">

        <section>
            <div class="ecology__slick__img">
                <img src="@/assets/foto/ecology_1.png" alt="ecology">
            </div>
        </section>

        <section>
            <div class="ecology__slick__img">
                <img src="@/assets/foto/ecology_2.png" alt="ecology">
            </div>
        </section>

        <section>
            <div class="ecology__slick__img">
                <img src="@/assets/foto/ecology_3.png" alt="ecology">
            </div>
        </section>

    </VueSlickCarousel>
 </template>


 <script>
 import VueSlickCarousel from "vue-slick-carousel";
 import "vue-slick-carousel/dist/vue-slick-carousel.css";
 export default {
     data(){
         return{
             settings: {
                 arrows: true,
                 dots: false,
                 infinite: false,
                 speed: 1000,
                 slidesToShow: 2.5,
                 autoplay:true,
                 responsive: [
                        {
                         breakpoint: 1100,
                         settings: {
                             slidesToShow: 1.5,
                             slidesToScroll: 1,
                            }
                        },

                        {
                        breakpoint: 750,
                        settings: {
                             slidesToShow: 1,
                             slidesToScroll: 1,
                            }
                        },

                        {
                        breakpoint: 550,
                        settings: {
                            slidesToScroll: 1,
                            speed:1500,
                            autoplayTimeout:1500,
                            fade:true
                            }
                        }
                ]
             },
         }
     },

     components:{
         VueSlickCarousel
     },
 }
 </script>
