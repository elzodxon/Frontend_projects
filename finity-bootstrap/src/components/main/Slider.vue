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
    <div class="container d-flex justify-content-center p-3">
      <div class="row">
        <div class="d-flex  justify-content-center mybtn col-12 ">
          <a href="" >
            <svg width="19" height="19" viewBox="0 0 19 19" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd" clip-rule="evenodd" d="M9.5 0C4.25125 0 0 4.25125 0 9.5C0 14.7488 4.25125 19 9.5 19C14.7488 19 19 14.7488 19 9.5C19 4.25125 14.7488 0 9.5 0ZM7.6 13.775L13.3 9.5L7.6 5.225V13.775ZM1.9 9.5C1.9 13.6895 5.3105 17.1 9.5 17.1C13.6895 17.1 17.1 13.6895 17.1 9.5C17.1 5.3105 13.6895 1.9 9.5 1.9C5.3105 1.9 1.9 5.3105 1.9 9.5Z" fill="white"/>
            </svg>
            <p class="ml-2">See Finity in Action</p>
          </a>
        </div>
      </div>
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
        "autoplay": true,
        "autoplaySpeed": 2000,
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

.mybtn{
  padding: 20px;
  height: 55px;
  background: #0F53FA;
  border-radius: 5px;

  a{
    display: flex;
    justify-content: center;
    font-size: 16px;
    font-style: normal;
    font-weight: 500;
    line-height: 20px;
    letter-spacing: 0px;
    color: #FFFFFF;
    text-decoration: none;
  }
}
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

@media screen and (max-width: 768px ){
  .row h2{
    font-size: 37px;
  }
}

</style>