<template>
  <footer class="footer">
      <div class="container">
        <ul class="flex">
          <li>
            <img src="../assets/imgs/Logodark.png" alt="">
            <h2 style="font-size: 16px;
                        font-style: normal;
                        font-weight: 400;
                        line-height: 28px;
                        letter-spacing: 0px;
                        text-align: left;
                        color: #8C97AC;"> Your ulitmate email solution to grow <br> business and engaging with future  customers and clients.</h2>
            <router-link to="/question"
                         style="font-size: 13px;
                          font-style: normal;
                          font-weight: 500;
                          line-height: 20px;
                          letter-spacing: 0px;
                          text-align: center;
                          width: 125px;
                          height: 45px;
                          padding: 20px;
                          background: #0F53FA;
">Ask a question</router-link>
          </li>
          <li>
            <ul class="flex" style="padding: 0 40px">
              <li>
                <ul>
                  <li>Community</li>
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
                <ul>
                  <li>About Us</li>
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
                <ul>
                  <li>Contacts</li>
                  <li>Feel free to get in touch with us via phone or send us a message.</li>
                  <li>
                    <a href="">+1-301-340-3946</a>
                  </li>
                  <li>
                    <a href="">info@finity.com</a>
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

.container{
  max-width: 1100px;
  margin: 0 auto;
  padding-top: 137px;
}
.flex{
  display: flex;
  justify-content: space-between;
}
  .footer{
    background: url("../assets/imgs/F.png");
    background-size: cover;
    height: 70vh;
  }

  a{
    text-decoration: none;
    color: white;
  }
</style>