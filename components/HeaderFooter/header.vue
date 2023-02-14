<template>

    <header>
        <div class="header">
            <section class="container">
                <div class="header__cart">
                    <div class="header__list">
                        <div class="header__logo">
                            <nuxt-link :to="localePath('/')">
                                <img src="@/assets/foto/logo.png" alt="logo">
                            </nuxt-link>
                        </div>

                        <ul class="header__menu" :class="{ header__burger__menu: burger }">
                            <li>
                                <nuxt-link :to="localePath('/about')" class="header__menu__link">{{ $t('aboutUs') }}</nuxt-link>
                            </li>

                            <li>
                                <nuxt-link :to="localePath('/partners')" class="header__menu__link">{{ $t('partners') }}</nuxt-link>
                            </li>

                            <li>
                                <nuxt-link :to="localePath('/contacts')" class="header__menu__link">{{ $t('contacts') }}</nuxt-link>
                            </li>
                        </ul>

                        <section class="header__locale__list">
                            <button class="header__button__burger" @click="burger = !burger">
                                <i class="fas fa-bars"></i>
                            </button>

                            <ul class="header__locales__cart">
                                <li @click="headerLocales = !headerLocales">
                                    {{ localeTitle }}

                                    <ul :class="{header__locales__menu : headerLocales}">
                                        <li v-for="(locale,index) in availableLocales" :key="index + locale.code">
                                            <button :class="{header__locales__active : locale.code === localeTitle}" @click.prevent="handleLangChange(locale.code)">{{ locale.code}}</button>
                                        </li>
                                    </ul>
                                </li>
                            </ul>
                        </section>

                    </div>
                </div>
                <div @click="burger = !burger" v-bind:class="{ header__burger__overflow: burger }"></div>
            </section>
        </div>
    </header>

</template>

<script>
export default {
    data(){
        return{
            burger:false,
            localeTitle:'',
            headerLocales:false
        }
    },
    computed:{
        availableLocales(){
            this.localeTitle = this.$i18n.loadedLanguages[0]
            return this.$i18n.locales
        }
    },

    methods:{
    handleLangChange(langCode) {
      this.$i18n.setLocale(langCode)
      this.localeTitle = langCode
    }
  }
}
</script>
