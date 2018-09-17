<template>
  <div class="wrapper">
    <swiper :items="items_one"/>
    <!--<swiper :items="items_two"/>-->
  </div>
</template>

<script>
  import Swiper from '@/components/Swiper'
  export default {
      components: {
          Swiper
      },
      data() {
          return {
              items_one: [
                  {
                      image_url: 'https://placeimg.com/640/480/any?1'
                  },
                  {
                      image_url: 'https://placeimg.com/640/480/any?2'
                  },
                  {
                      image_url: 'https://placeimg.com/640/480/any?3'
                  }
              ],
              items_two: [
                  {
                      image_url: 'https://placeimg.com/640/480/any?4'
                  },
                  {
                      image_url: 'https://placeimg.com/640/480/any?5'
                  },
                  {
                      image_url: 'https://placeimg.com/640/480/any?6'
                  }
              ]
          }
      }
  }
</script>