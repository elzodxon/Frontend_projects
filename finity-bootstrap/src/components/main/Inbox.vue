<template>
  <div class="container">
    <div class="row">
      <div class="col-lg-6 col-md-6 col-sm-12 ">
        <img src="/assets/imgs/inbox.png" class="img-fluid" alt="">
      </div>
      <div class="col-lg-5 col-sm-12 col-md-6  d-flex justify-content-center flex-column offset-lg-1  content">
       <div>
         <h1>Work anywhere, with any device</h1>
         <p>These companies release their own versions of the operating systems with minor changes, and yet always with
           the same bottom line. </p>
         <a href="">
           <img src="/assets/imgs/applestore.png" class="img-fluid" alt="">
         </a>
         <a href="">
           <img src="/assets/imgs/playstore.png" class="img-fluid" alt="">
         </a>
       </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

.content h1{
  font-size: 48px;
  font-style: normal;
  font-weight: 700;
  line-height: 56px;
  letter-spacing: -0.8275861740112305px;
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

@media screen and (max-width: 1000px){
  .content h1{
    font-size: 38px;
    line-height: 40px;
    margin-bottom: 20px;
  }
  .content p{
    margin-bottom: 18px;
  }
}
</style>