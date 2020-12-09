<template>
  <div class="container">
    <div class="container-wrapper">
      <h1>Solution made for you</h1>
      <p>These companies release their own versions of the operating <br> systems with minor changes, and yet always.</p>
    </div>
    <SliderC/>

  </div>
</template>

<script>

import SliderC from "@/components/SliderC"

export default {
  components: {
    SliderC
  }
}
</script>

<style scoped>
.container-wrapper{
  margin-bottom: 50px;
}

.container h1 {
  font-size: 48px;
  font-style: normal;
  font-weight: 700;
  line-height: 56px;
  letter-spacing: -0.8275861740112305px;
  text-align: center;
  color: #1D293F;
  margin-bottom: 39px;
}

.container p {
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 32px;
  letter-spacing: 0px;
  text-align: center;
  color: #7C8087;
}
</style>