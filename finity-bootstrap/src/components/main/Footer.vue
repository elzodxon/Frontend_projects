<template>
  <footer class="p-5">
    <div class="container ">
      <img src="/assets/imgs/yellow.png" alt="">

      <div class="row">
        <div class="col-lg-5 col-md-12">
          <img src="/assets/imgs/Logodark.png" alt="">
          <h2 class="motto"> Your ulitmate email solution to grow <br> business and engaging with future
            customers and clients.</h2>
          <router-link to="/question" class="ask-btn">Ask a question</router-link>
        </div>

        <ul class="col-lg-2 col-md-4 col-sm-2">
          <li class="footer-top">Community</li>
          <li class="footer-link">
            <router-link to="/for-talents">For talents</router-link>
          </li>
          <li class="footer-link">
            <router-link to="/for-companies">For companies</router-link>
          </li>
          <li class="footer-link">
            <router-link to="/facebook">Facebook Group</router-link>
          </li>
          <li class="footer-link">
            <router-link to="/faq">FAQ</router-link>
          </li>
        </ul>

        <ul class="col-lg-2 col-md-4 col-sm-2">
          <li class="footer-top">About Us</li>
          <li class="footer-link">
            <router-link to="/team">Meet the team</router-link>
          </li>
          <li class="footer-link">
            <router-link to="/our-story">Our story</router-link>
          </li>
          <li class="footer-link">
            <router-link to="/career">Career</router-link>
          </li>
        </ul>

        <ul class="col-lg-2 col-md-4 col-sm-2">
          <li class="footer-top">Contacts</li>
          <li class="footer-link">Feel free to get in touch with us via phone or send us a message.</li>
          <li>
            <a class="brown" href="">+1-301-340-3946</a> <br>
            <a class="brown" href="">info@finity.com</a>
          </li>
        </ul>
      </div>


    </div>
  </footer>
</template>

<style scoped>

a {
  text-decoration: none;
}

footer {
  background: #1D293F;
}

.footer-top {
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 32px;
  letter-spacing: 0px;
  color: #8C97AC;
}

.footer-link {
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 42px;
  letter-spacing: 0px;
  color: #E9F7FE !important;
}

.footer-link a {
  text-decoration: none;
  color: #E9F7FE !important;
}

.col-2 li:hover {
  text-decoration: underline;
}

.motto {
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 28px;
  letter-spacing: 0px;
  color: #8C97AC;
  margin-top: 30px;
}

.brown{
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 28px;
  letter-spacing: 0px;
  color: #FFD166 !important;
}

.ask-btn{
  display: flex;
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  letter-spacing: 0px;
  text-align: center;
  color: #E9F7FE;
  background: #0F53FA;
  border-radius: 5px;
  padding: 10px;
  height: 45px;
  width: 125px;
  align-items: center;
  justify-content: center;
}

@media screen and (max-width: 968px){
  .row{
    flex-direction: column;
  }

}


@media screen and (max-width: 910px){
  ul li{
    width: 200px;
  }

  .motto{
    width: 300px;
  }
}
</style>