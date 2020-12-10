<template>
  <div class="home">
      <Header/>
      <Companies/>
      <Slider/>
  </div>
</template>

<script>
// @ is an alias to /src

import Header from "@/components/header/Header";
import Companies from "@/components/main/Companies";
import Slider from "@/components/main/Slider"
export default {
  name: 'Home',
  components: {
    Companies,
    Header,
    Slider
  }
}
</script>
