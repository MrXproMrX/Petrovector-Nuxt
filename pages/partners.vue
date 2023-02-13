<template>
    <section>

        <!-- partners start -->

        <div class="partners">
            <div class="partners__item__title">
                <section class="container">
                    <h2 class="activities__title__h2">{{ $t('partners') }}</h2>
                </section>
            </div>

            <section class="container">
                <div class="partners__cart">
                    <partnersList :partnersList="partnersList"></partnersList>
                </div>
            </section>
        </div>

        <!-- partners end -->

    </section>
</template>

<script>
import partnersList from '~/components/partners/partnersList.vue';
import partnersListApi from '~/data/partnersListApi';
export default {
    data(){
        return{
            partnersList:partnersListApi
        }
    },

    components:{
        partnersList
    }
}
</script>

<style scoped>
.partners__item__title{
    background-image: url(@/assets/foto/partners_fon.png);
}
</style>
