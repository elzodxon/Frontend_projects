<template>
  <footer class="footer">
    <div class="container">
      <ul class="flex">
        <li>
          <img src="../assets/imgs/Logodark.png" alt="">
          <h2> Your ulitmate email solution to grow <br> business and engaging with future
            customers and clients.</h2>
          <router-link to="/question" class="ask-btn">Ask a question</router-link>
        </li>
        <li>
          <ul class="flex" style="padding: 0 20px">
            <li>
              <ul class="footer-list">
                <li class="footer-top">Community</li>
                <li>
                  <router-link to="/for-talents">For talents</router-link>
                </li>
                <li>
                  <router-link to="/for-companies">For companies</router-link>
                </li>
                <li>
                  <router-link to="/facebook">Facebook Group</router-link>
                </li>
                <li>
                  <router-link to="/faq">FAQ</router-link>
                </li>
              </ul>
            </li>
            <li>
              <ul class="footer-list">
                <li class="footer-top">About Us</li>
                <li>
                  <router-link to="/team">Meet the team</router-link>
                </li>
                <li>
                  <router-link to="/our-story">Our story</router-link>
                </li>
                <li>
                  <router-link to="/career">Career</router-link>
                </li>
              </ul>
            </li>
            <li>
              <ul class="footer-list">
                <li class="footer-top">Contacts</li>
                <li>Feel free to get in touch with us via phone or send us a message.</li>
                <li>
                  <a class="brown" href="">+1-301-340-3946</a> <br>
                  <a class="brown" href="">info@finity.com</a>
                </li>

              </ul>
            </li>
          </ul>
        </li>
      </ul>
    </div>
  </footer>
</template>


<script>

</script>

<style scoped>

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding-top: 137px;
}

.flex {
  display: flex;
  justify-content: space-between;
}

.footer {
  background: url("../assets/imgs/F.png");
  background-size: cover;
  height: 70vh;
}

a {
  text-decoration: none;
  color: white;
}

h2{
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 28px;
  letter-spacing: 0px;
  text-align: left;
  color: #8C97AC;
  margin-bottom: 35px;
  margin-top: 25px;
}
.ask-btn {
  font-size: 13px;
  font-weight: 500;
  line-height: 20px;
  letter-spacing: 0px;
  text-align: center;
  width: 125px;
  height: 45px;
  padding: 20px;
  background: #0F53FA;
}

.footer-list{
  width: 100px;
}

.footer-list:last-child{
  width: 300px !important;
}
.footer-list li:not(first-child){
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 42px;
  letter-spacing: 0px;
  text-align: left;
  color: #E9F7FE;
  margin-left: 50px;
}

.footer-top{
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 32px;
  letter-spacing: 0px;
  color: #8C97AC;
}

.brown{
  color: #FFD166;
}
</style>