<template>
  <div class="container">
    <div class="row">
      <img src="../assets/imgs/inbox.png" alt="">
      <div class="content">
        <h1>Work anywhere, <br> with any device</h1>
        <p>These companies release their own versions of the operating systems with minor changes, and yet always with
          the same bottom line. </p>
        <a href="">
          <img src="../assets/imgs/applestore.png" alt="">
        </a>
        <a href="">
          <img src="../assets/imgs/playstore.png" alt="">
        </a>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style scoped>
.container {
  max-width: 1050px;
  margin: 0 auto;
}

.row {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.content h1{
  margin-bottom: 40px;
}

.content p{
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 32px;
  letter-spacing: 0px;
  color: #7C8087;
  margin-bottom: 56px;
}

.content img{
  margin-bottom: 15px;
}
</style>