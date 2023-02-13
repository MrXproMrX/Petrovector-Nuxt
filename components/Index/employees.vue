<template>
   <VueSlickCarousel v-bind="settings" class="employees__list">
        <div class="employees__item">
            <div class="employees__img">
                <img src="@/assets/foto/person_1.png" alt="employees">
            </div>
            <h2 class="employees__title__h2">{{ $t('employeesName1') }}</h2>
            <div class="employees__text">{{ $t('employeesText1') }}</div>
        </div>

        <div class="employees__item">
            <div class="employees__img">
                <img src="@/assets/foto/person_2.png" alt="employees">
            </div>
            <h2 class="employees__title__h2">{{ $t('employeesName2') }}</h2>
            <div class="employees__text">{{ $t('employeesText2') }}</div>
        </div>

        <div class="employees__item">
            <div class="employees__img">
                <img src="@/assets/foto/person_3.png" alt="employees">
            </div>
            <h2 class="employees__title__h2">{{ $t('employeesName3') }}</h2>
            <div class="employees__text">{{ $t('employeesText3') }}</div>
        </div>

        <div class="employees__item">
            <div class="employees__img">
                <img src="@/assets/foto/person_4.png" alt="employees">
            </div>
            <h2 class="employees__title__h2">{{ $t('employeesName4') }}</h2>
            <div class="employees__text">{{ $t('employeesText4') }}</div>
        </div>

        <div class="employees__item">
            <div class="employees__img">
                <img src="@/assets/foto/person_5.png" alt="employees">
            </div>
            <h2 class="employees__title__h2">{{ $t('employeesName5') }}</h2>
            <div class="employees__text">{{ $t('employeesText5') }}</div>
        </div>

        <div class="employees__item">
            <div class="employees__img">
                <img src="@/assets/foto/person_6.png" alt="employees">
            </div>
            <h2 class="employees__title__h2">{{ $t('employeesName6') }}</h2>
            <div class="employees__text">{{ $t('employeesText6') }}</div>
        </div>

        <div class="employees__item">
            <div class="employees__img">
                <img src="@/assets/foto/person_7.png" alt="employees">
            </div>
            <h2 class="employees__title__h2">{{ $t('employeesName7') }}</h2>
            <div class="employees__text">{{ $t('employeesText7') }}</div>
        </div>

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
                    slidesToShow: 3,
                    slidesToScroll: 1,
                     responsive: [
                   {
                  breakpoint: 1200,
                  settings: {
                  slidesToShow: 2,
                  slidesToScroll: 1,
                  infinite: true,
                  dots: false
                  }
                },
                 {
                  breakpoint: 650,
                  settings: {
                  slidesToShow: 1,
                 slidesToScroll: 1
                  }
                 },
               ]
            },
        }
    },

    components:{
        VueSlickCarousel
    },
}
</script>
