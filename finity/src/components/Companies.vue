<template>
  <div class="container">
    <div class="wrapper">
      <router-link to="/geekwire">
        <img src="../assets/imgs/geekwire.svg" alt="">
      </router-link>
      <router-link to="/slack">
        <img src="../assets/imgs/slack.svg" alt="">
      </router-link>
      <router-link to="/envato">
        <img src="../assets/imgs/envato.svg" alt="">
      </router-link>
      <router-link to="/usatoday">
        <img src="../assets/imgs/usatoday.svg" alt="">
      </router-link>
      <router-link to="/forbes">
        <img src="../assets/imgs/forbes.svg" alt="">
      </router-link>

    </div>
  </div>
</template>

<script>

</script>

<style scoped>
.container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 50px;
}

.wrapper img:hover {
  color: #7C8087;
}

.wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}


@media screen and (max-width: 550px){
  .wrapper img{
    margin: 0 auto;
    width: 100%;
  }
}

</style>