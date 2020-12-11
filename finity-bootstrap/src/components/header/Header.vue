<template>
  <div class="header">
      <b-navbar toggleable="lg" type="light">
        <b-navbar-brand href="#">
          <img src="assets/logo.png" alt="">
        </b-navbar-brand>

        <b-navbar-toggle style="outline: none; border: none" target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>

          <b-navbar-nav class="ml-auto">

            <b-navbar-nav>
              <b-nav-item class="ml-3">
                <router-link to="/demos">Demos</router-link>
              </b-nav-item>
              <b-nav-item class="ml-3">
                <router-link to="/pages">Pages</router-link>
              </b-nav-item>
              <b-nav-item class="ml-3">
                <router-link to="/support">Support</router-link>
              </b-nav-item>
              <b-nav-item class="ml-3">
                <router-link class="trial-btn"  to="/trial">Start 14 Days Free Trial</router-link>
              </b-nav-item>
            </b-navbar-nav>

          </b-navbar-nav>
        </b-collapse>
      </b-navbar>

      <main class="main">
        <div class="main-wrapper">
          <img style="display: none" class="img-fluid" src="/assets/App.png" alt="">
          <h1>More than your regular email inbox</h1>
          <h4>We’ve helped over 25,000 individuals and companies to grow their business successfully.</h4>
          <router-link class="main-btn" to="/register">Start 14 days free trial</router-link>
          <p>No credit card required</p>
        </div>
      </main>



  </div>
</template>


<script>

</script>

<style lang="scss" scoped>

.header{
  background-position: bottom  center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
  background-image: url("/assets/imgs/BG.png");
}
a{
  text-decoration: none;
  color: black;
}

.trial-btn{
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #0F53FA;
  border-radius: 5px;
  height: 45px;
  width: 170px;
  color: white !important;
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  text-align: center;
}


/* Main section */
.main {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 100px;
}

.main-wrapper {
  width: 500px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.main h1 {
  font-size: 58px;
  font-style: normal;
  font-weight: 700;
  line-height: 64px;
  letter-spacing: -1px;
  text-align: center;
  color: #1D293F;
  margin-bottom: 40px;
}

.main h4 {
  font-size: 21px;
  font-style: normal;
  font-weight: 400;
  line-height: 30px;
  letter-spacing: 0px;
  text-align: center;
  color: #7C8087;
  margin-bottom: 40px;

}

.main p {
  font-size: 13px;
  font-style: normal;
  font-weight: 400;
  line-height: 20px;
  letter-spacing: 0px;
  text-align: center;
  color: #8C97AC;
}

.main-btn {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 16px;
  font-weight: 500;
  line-height: 20px;
  background-color: #0F53FA;
  border-radius: 5px;
  height: 55px;
  width: 217px;
  color: white;
  text-decoration: none;
  /*position: relative;*/
  /*left: 25%;*/
  margin-bottom: 15px;
}


/* Media queries */

@media only screen and (max-width: 950px){
  .header{
    background-image: none;
    background: #F7F8FA;
    height: 70vh;
  }
}

@media only screen and (max-width: 550px) {
  .main-wrapper{
    width: 100%;
    h1{
      font-size: 40px !important;
      line-height: 45px !important;
      margin-bottom: 20px;
      width: 80%;
    }
    h4{
      font-size: 17px;
      width: 80%;
      margin-bottom: 20px;
    }
  }
}

</style>