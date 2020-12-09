<template>
  <div class="container">
    <nav>
      <ul class="nav-list flex">
        <li>
          <router-link to="/">
            <img class="nav-logo" src="../assets/imgs/logo.png" alt="">
          </router-link>
        </li>
        <li>
          <ul class="nav-list__right flex">
            <li>
              <router-link class="decoration" to="/demos">Demos</router-link>
            </li>
            <li>
              <router-link class="decoration" to="/pages">Pages</router-link>
            </li>
            <li>
              <router-link class="decoration" to="support">Support</router-link>
            </li>
            <li class="trial-btn">
              <router-link class="decoration" to="/register"> Start 14 days free trial</router-link>
            </li>
          </ul>
        </li>
      </ul>
    </nav>
    <main class="main">
      <div class="main-wrapper">
        <h1>More than your regular email inbox</h1>
        <h4>We’ve helped over 25,000 individuals and companies to grow their business successfully.</h4>
        <router-link class="main-btn" to="/register">Start 14 days free trial</router-link>
        <p>No credit card required</p>
      </div>

    </main>

  </div>

</template>

<script>
export default {
  name: 'Navbar',

}
</script>

<style scoped>
.container {
  background: url("../assets/imgs/BG.png");
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
  padding: 30px 38px;
}
.decoration{
  text-decoration: none;
  color: black;
  font-size: 16px;
  font-weight: 400;
  line-height: 28px;
}
.flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
router-link{
  text-decoration: none;
}
.nav-list__right li{
  margin-right: 44px;
}
/* Trial button */
.trial-btn{
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #0F53FA;
  border-radius: 5px;
  height: 45px;
  width: 170px;
}
.trial-btn .decoration{
  color: white !important;
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  text-align: center;
}

/* Main section */
.main{
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 125px;
}

.main-wrapper{
  width: 500px;
  text-align: center;
}
.main h1{
  font-size: 58px;
  font-style: normal;
  font-weight: 700;
  line-height: 64px;
  letter-spacing: -1px;
  text-align: center;
  color: #1D293F ;
  margin-bottom: 40px;
}

.main h4{
  font-size: 21px;
  font-style: normal;
  font-weight: 400;
  line-height: 30px;
  letter-spacing: 0px;
  text-align: center;
  color:  #7C8087;
  margin-bottom: 40px;

}

.main p{
  font-size: 13px;
  font-style: normal;
  font-weight: 400;
  line-height: 20px;
  letter-spacing: 0px;
  text-align: center;
  color: #8C97AC;
}

.main-btn{
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
  position: relative;
  left: 25%;
  margin-bottom: 15px;
}
</style>