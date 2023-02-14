<template>
    <section>
        <div class="contacts_in">
            <section class="container">
                <div class="contacts_in__cart">
                    <div class="contacts_in__list">
                        <div class="contacts_in__item">
                            <h2 class="activities__title__h2">Contacts</h2>

                            <div class="contacts__item">
                                <h4>{{ $t('geneva') }}</h4>
                            </div>

                            <div class="contacts__item">
                                <h3>{{ $t('petrovector') }}</h3>
                            </div>

                            <div class="contacts__item">
                                <h3>{{ $t('tel') }}</h3>
                            </div>

                        </div>

                        <div class="contacts_in__item__map">
                            <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d1461.8409469391293!2d74.59988978382712!3d42.879557920359915!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x389eb7e74697b7a5%3A0xb625d929c04e872e!2z0J_QsNGA0Log0J_QsNC90YTQuNC70L7QstCw!5e0!3m2!1sru!2s!4v1676359871946!5m2!1sru!2s" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                        </div>
                    </div>
                </div>
            </section>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style scoped>
.contacts_in{
    background-image: url(@/assets/foto/map_Fon.png);
}
</style>
