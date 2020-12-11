<template>
  <div class="home">
    <Header/>
    <Companies/>
    <Slider/>
    <Inbox/>
    <Testimonials/>
    <Price/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src

import Header from "@/components/header/Header";
import Companies from "@/components/main/Companies";
import Slider from "@/components/main/Slider"
import Testimonials from '@/components/main/Testimonials'
import Price from "@/components/main/Price";
import Footer from "@/components/main/Footer";
import Inbox from "@/components/main/Inbox";

export default {
  name: 'Home',
  components: {
    Inbox,
    Footer,
    Price,
    Companies,
    Header,
    Slider,
    Testimonials,
  }
}
</script>
