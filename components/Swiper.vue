<template>
    <div class="swiper" v-swiper:mySwiper="swiperOptions">
        <div class="swiper-wrapper">
            <div class="swiper-slide" v-for="item in items">
                <img :src="item.image_url">
            </div>
        </div>
        <div class="swiper-pagination"></div>
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>
    </div>
</template>

<script>
    export default {
        props: ['items'],
        data() {
            return {
                swiperOptions: {
                    pagination: {
                        el: '.swiper-pagination',
                        clickable: true
                    },
                    navigation: {
                        nextEl: '.swiper-button-next',
                        prevEl: '.swiper-button-prev'
                    },
                    loop: true,
                    slidesPerView: 'auto',
                    loopedSlides: 10
                }
            }
        }
    }
</script>

<style>
    .swiper-slide {
        width: auto;
    }
</style>