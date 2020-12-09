<template>
  <div class="home">
      <Navbar/>
      <Companies/>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar";
import Companies from "@/components/Companies"
export default {
  name: 'Home',
  components: {
    Navbar,
    Companies
  }
}
</script>


<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700;900&display=swap');

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body{
  font-family: 'Roboto', sans-serif;

}
</style>
