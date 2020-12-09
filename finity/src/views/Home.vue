<template>
  <div class="home">
    <Navbar/>
    <Companies/>
<!--    <Solutions/>-->
<!--    <Content/>-->
<!--    <Inbox/>-->
<!--    <Testimonials/>-->
<!--    <Footer/>-->
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar";
import Companies from "@/components/Companies"
// // import Solutions from "@/components/Solutions"
// /*
// import Content from '@/components/Content'
// */
// import Inbox from '@/components/Inbox'
// import Testimonials from '@/components/Testimonials'
// import Footer from '@/components/Footer'
export default {
  name: 'Home',
  components: {
    Navbar,
    Companies,
    // Solutions,
    // // Content,
    // Inbox,
    // Testimonials,
    // Footer
  }
}
</script>


<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700;900&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Roboto', sans-serif;

}
</style>
