<template>
    <section>
        <!-- about start -->

        <div class="about">
            <section class="container">
                <div class="about__cart">
                    <div class="about__list">
                        <h2 class="activities__title__h2">{{ $t('aboutTitle') }}</h2>

                        <div class="about__text" v-html="($t('aboutText'))"></div>

                        <a href="@/assets/foto/Petrovector_SA_2022_V2.pdf" download class="about__link">
                            {{ $t('aboutLink') }}
                        </a>
                    </div>
                </div>
            </section>
        </div>

        <!-- about end -->


        <!-- priorities start -->

        <div class="priorities">
            <section class="container">
                <div class="priorities__cart">
                   <prioritiesListVue></prioritiesListVue>
                </div>
            </section>
        </div>

        <!-- priorities end -->


        <!-- charity start -->

        <div class="charity">
            <section class="container">
                <div class="charity__cart">
                    <div class="charity__list">
                        <h2 class="activities__title__h2">{{$t('charityTitle')}}</h2>
                        <div class="charity__taxt">
                            <p>
                                {{ $t('charityText') }}
                            </p>
                        </div>
                    </div>
                </div>
            </section>
        </div>

        <!-- charity end -->


        <!-- ecology start -->

        <div class="ecology">
            <section class="container">
                <div class="ecology__cart">

                    <h2 class="activities__title__h2">{{ $t('ecologyTitle') }}</h2>

                    <div class="ecology__list">
                        <div class="ecology__item">
                            <div class="ecology__list__text">
                                <p>
                                    {{ $t('ecologyText_1') }}
                                </p>
                            </div>

                            <div class="ecology__text">
                                <p>
                                    {{ $t('ecologyText_2') }}
                                </p>
                            </div>
                        </div>

                        <ecologySlickVue></ecologySlickVue>
                    </div>
                </div>
            </section>
        </div>

        <!-- ecology end -->


        <!-- social start -->

        <div class="social">
            <section class="container">
                <div class="social__cart">
                    <h2 class="activities__title__h2">{{ $t('socialTitle') }}</h2>
                    <div class="social__text">
                        <p>
                            {{ $t('socialTextTop') }}
                        </p>
                    </div>

                    <div class="social__list">
                        <div class="social__item">
                            <div class="social__item__number">1</div>
                            <section>
                                <h3 class="social__title__h3">{{ $t('socialTitle_1') }}</h3>
                                <div class="social__cart__text">
                                    {{ $t('socialText_1') }}
                                </div>
                            </section>
                        </div>

                        <div class="social__item">
                            <div class="social__item__number">2</div>
                            <section>
                                <h3 class="social__title__h3">{{ $t('socialTitle_2') }}</h3>
                                <div class="social__cart__text">
                                    {{ $t('socialText_2') }}
                                </div>
                            </section>
                        </div>

                        <div class="social__item">
                            <div class="social__item__number">3</div>
                            <section>
                                <h3 class="social__title__h3">{{ $t('socialTitle_3') }}</h3>
                                <div class="social__cart__text">
                                    {{ $t('socialText_3') }}
                                </div>
                            </section>
                        </div>

                        <div class="social__item">
                            <div class="social__item__number">4</div>
                            <section>
                                <h3 class="social__title__h3">{{ $t('socialTitle_4') }}</h3>
                                <div class="social__cart__text">
                                    {{ $t('socialText_4') }}
                                </div>
                            </section>
                        </div>

                        <div class="social__item">
                            <div class="social__item__number">5</div>
                            <section>
                                <h3 class="social__title__h3">{{ $t('socialTitle_5') }}</h3>
                                <div class="social__cart__text">
                                    {{ $t('socialText_5') }}
                                </div>
                            </section>
                        </div>

                        <div class="social__item">
                            <div class="social__item__number">6</div>
                            <section>
                                <h3 class="social__title__h3">{{ $t('socialTitle_6') }}</h3>
                                <div class="social__cart__text">
                                    {{ $t('socialText_6') }}
                                </div>
                            </section>
                        </div>
                    </div>

                    <div class="social__text__list">
                        <p>
                            {{ $t('socialTextBootom') }}
                        </p>
                    </div>
                </div>
            </section>
        </div>

        <!-- social end -->
    </section>
</template>

<style scoped>
.about{
    background-image: url(@/assets/foto/about_fon.png);
}
</style>

<script>
import prioritiesListVue from '~/components/about/prioritiesList.vue';
import ecologySlickVue from '~/components/about/ecologySlick.vue';
export default {
   components:{
    prioritiesListVue,
    ecologySlickVue
   }
}
</script>
