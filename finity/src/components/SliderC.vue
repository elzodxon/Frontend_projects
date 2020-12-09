<template>
  <VueSlickCarousel v-bind="settings">
    <div class="swiper-wrapper">
      <img src="../assets/imgs/oval3.png" alt="">
      <div class="infor">
        <h2>Team Collaboration</h2>
        <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
      </div>
    </div>
    <div class="swiper-wrapper">
      <img src="../assets/imgs/oval3.png" alt="">
      <div class="infor">
        <h2>Team Collaboration</h2>
        <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
      </div>
    </div>
    <div class="swiper-wrapper">
      <img src="../assets/imgs/oval3.png" alt="">
      <div class="infor">
        <h2>Team Collaboration</h2>
        <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
      </div>
    </div>
    <div class="swiper-wrapper">
      <img src="../assets/imgs/oval3.png" alt="">
      <div class="infor">
        <h2>Team Collaboration</h2>
        <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
      </div>
    </div>
    <div class="swiper-wrapper">
      <img src="../assets/imgs/oval3.png" alt="">
      <div class="infor">
        <h2>Team Collaboration</h2>
        <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
      </div>
    </div>
    <div class="swiper-wrapper">
      <img src="../assets/imgs/oval3.png" alt="">
      <div class="infor">
        <h2>Team Collaboration</h2>
        <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
      </div>
    </div>
    <div class="swiper-wrapper">
      <img src="../assets/imgs/oval3.png" alt="">
      <div class="infor">
        <h2>Team Collaboration</h2>
        <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
      </div>
    </div>

  </VueSlickCarousel>
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
        "infinite": true,
        "initialSlide": 3,
        "speed": 500,
        "centerMode": true,
        "centerPadding": "30px",
        "focusOnSelect": true,
        "slidesToShow": 5,
      },
    }
  },
}
</script>

<style scoped>
  .swiper-wrapper{
    display: flex !important;
    align-items: flex-start;
    background: #F7F8FA;
    height: 158px !important;
    width: 350px !important;
    padding: 20px;
  }

  .swiper-wrapper h2{
    font-size: 21px;
    font-style: normal;
    font-weight: 700;
    line-height: 34px;
    letter-spacing: 0px;
  }

  .swiper-wrapper h4{
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 28px;
    letter-spacing: 0px;
  }
</style>