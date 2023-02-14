<template>
    <div class="partners__list">
        <div class="partners__item" v-for="(item,i) in partnersList" :key="i">
            <div class="partners__item__logo">
                <div class="partners__img">
                    <img :src="item.imgs" :alt="item.title">
                </div>
            </div>
            <h3 class="partners__title__h3">{{ item.title }}</h3>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        partnersList:{
            type:Array,
            required: true,
            default: () => []
        }
    }
}
</script>
