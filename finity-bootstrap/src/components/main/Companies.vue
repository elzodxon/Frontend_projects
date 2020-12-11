<template>
  <div class="container">
    <VueSlickCarousel v-bind="settings" class="row p-4">
      <div class="col-lg-3 col-md-2 col-sm-2">
        <img src="/assets/imgs/geekwire.svg" alt="">
      </div>
      <div class="col-lg-2 col-md-2 col-sm-2">
        <img src="/assets/imgs/slack.svg" alt="">
      </div>
      <div class="col-lg-2 col-md-2 col-sm-2">
        <img src="/assets/imgs/envato.svg" alt="">
      </div>
      <div class="col-lg-2 col-md-2 col-sm-2">
        <img src="/assets/imgs/usatoday.svg" alt="">
      </div>
      <div class="col-lg-3 col-md-2 col-sm-2">
        <img src="/assets/imgs/forbes.svg" alt="">
      </div>
    </VueSlickCarousel>


  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
  name: 'MyComponent',
  components: { VueSlickCarousel },

  data() {
    return {

      settings: {
        "infinite": false,
        "speed": 500,
        "slidesToShow": 5,
        "slidesToScroll": 1,
        "initialSlide": 0,
        "arrows": false,
        "responsive": [
          {
            "breakpoint": 1024,
            "settings": {
              "slidesToShow": 3,
              "slidesToScroll": 2,
              "infinite": true,
            }
          },
          {
            "breakpoint": 600,
            "settings": {
              "slidesToShow": 2,
              "slidesToScroll": 2,
              "initialSlide": 2
            }
          },
          {
            "breakpoint": 480,
            "settings": {
              "slidesToShow": 2,
              "slidesToScroll": 1
            }
          }
        ]
      }
    }
  },
}
</script>
<style scoped>

</style>