<template>
  <div>
    <div class="container p-5">
      <div class="row d-flex align-items-center flex-column">
        <h2>Solution made for you</h2>
        <h3 class="text-center">These companies release their own versions of the operating <br> systems with minor changes, and yet always.</h3>
      </div>
    </div>
    <div class="slick_slide">
      <VueSlickCarousel v-bind="settings">
        <div class="swiper-wrapper">
          <img src="/assets/imgs/oval3.png" alt="" class="mr-2">
          <div class="infor">
            <h2>Find Leads</h2>
            <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
          </div>
        </div>
        <div class="swiper-wrapper">
          <img src="/assets/imgs/oval3.png" alt="" class="mr-2">
          <div class="infor">
            <h2>Team Collaboration</h2>
            <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
          </div>
        </div>
        <div class="swiper-wrapper">
          <img src="/assets/imgs/oval3.png" alt="" class="mr-2">
          <div class="infor">
            <h2>Instant Chat</h2>
            <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
          </div>
        </div>
        <div class="swiper-wrapper">
          <img src="/assets/imgs/oval3.png" alt="" class="mr-2">
          <div class="infor">
            <h2>Media manager</h2>
            <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
          </div>
        </div>
        <div class="swiper-wrapper">
          <img src="/assets/imgs/oval3.png" alt="" class="mr-2">
          <div class="infor">
            <h2>Dedicated Storage</h2>
            <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
          </div>
        </div>
        <div class="swiper-wrapper">
          <img src="assets/imgs/oval3.png" alt="" class="mr-2">
          <div class="infor">
            <h2>Team Collaboration</h2>
            <h4>We’ve helped over 2,500 job seekers to get into the most popular tech teams.</h4>
          </div>
        </div>


      </VueSlickCarousel>
    </div>
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

        "infinite": true,
        "initialSlide": 3,
        "speed": 500,
        "centerMode": true,
        "centerPadding": "20px",
        "focusOnSelect": true,
        "slidesToShow": 5,
        "variableWidth": true,
        "responsive":[
          {
              "breakpoint": 1220,
              "settings":{
                "slidesToShow": 4,
                "infinite": true,
                "initialSlide": 3,
                "speed": 1000,
                "centerMode": true,
                "centerPadding": "20px",
                "focusOnSelect": true,

              }
          },
          {
            "breakpoint": 1020,
            "settings":{
              "slidesToShow": 3,
              "infinite": true,
              "initialSlide": 1,
              "speed": 1000,
              "centerMode": true,
              "centerPadding": "20px",
              "focusOnSelect": true,

            }
          },
          {
            "breakpoint": 950,
            "settings":{
              "slidesToShow": 2,
              "infinite": true,
              "initialSlide": 1,
              "speed": 1000,
              "centerMode": true,
              "centerPadding": "20px",
              "focusOnSelect": true,

            }
          },
          {
            "breakpoint": 550,
            "settings":{
              "slidesToShow": 1,
              "infinite": true,
              "initialSlide": 1,
              "speed": 1000,
              "centerMode": true,
              "centerPadding": "20px",
              "focusOnSelect": true,

            }
          },
        ]
      },
    }
  },
}
</script>

<style lang="scss" scoped>

/* Top styles */

.row{
  h2{
    font-size: 48px;
    font-style: normal;
    font-weight: 700;
    line-height: 56px;
    letter-spacing: -0.8275861740112305px;
    color: #1D293F;
  }

  h3{
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: 32px;
    letter-spacing: 0px;
    color: #7C8087;

  }
}

/* Slick Slider */
.slick_slide{
  overflow: hidden;
}
.swiper-wrapper{
  display: flex !important;
  align-items: flex-start;
  background: #ECEFF4;
  width: 350px !important;
  padding: 20px;
  margin-right: 70px;
  border-radius: 10px;
  cursor: pointer;
  .slick-current {
    position: relative;
  }
}

.swiper-wrapper h2{
  font-size: 21px;
  font-style: normal;
  font-weight: 700;
  line-height: 34px;
  letter-spacing: 0px;
  color: #1D293F;
}

.swiper-wrapper h4{
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 28px;
  letter-spacing: 0px;
  color: #7C8087;
}
.swiper-wrapper:focus{
  outline: none;
}


@media only screen and (max-width: 550px) {
  .swiper-wrapper{
    margin-right: 95px;
    margin-left: 50px;
  }
}

</style>