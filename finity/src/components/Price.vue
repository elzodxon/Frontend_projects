<template>
  <div class="container">
    <div class="items">
      <h2>Choose the right <br> plan for your finity</h2>
      <div class="btn-change">
        <button
            :class="{
           active: type === 'yearly',
            }"
            @click="type = 'yearly'"
        >
          Yearly
        </button>
        <button
            :class="{
           active: type === 'monthly',
            }"
            @click="type = 'monthly'"
        >
          Monthly
        </button>
      </div>

    </div>

    <ul class="row">
      <li>
         Starter_
      </li>
      <li>
        <ul>
          <li>10GB Storage</li>
          <li>15 Accounts</li>
          <li>1,000 Connections</li>
        </ul>
      </li>
      <li>
        <ul>
          <li v-if="type === 'yearly'">228$</li>
          <li v-else>30$</li>
          <li v-if="type === 'yearly'">$19 per month</li>
          <li v-else></li>
          <li v-if="type=== 'yearly'" >billed yearly</li>
          <li v-else>billed monthly</li>
        </ul>
      </li>
      <li>
        <BTN/>
      </li>
    </ul>
    <hr>
    <ul class="row">
      <li>
        Standard
      </li>
      <li>
        <ul>
          <li>100GB Storage</li>
          <li>50 Accounts</li>
          <li>5,000 Connections</li>
        </ul>
      </li>
      <li>
        <ul>
          <li v-if="type === 'yearly'">468$</li>
          <li v-else>50$</li>
          <li v-if="type === 'yearly'">$39 per month</li>
          <li v-else></li>
          <li v-if="type==='yearly'">billed yearly</li>
          <li v-else>billed monthly</li>
        </ul>
      </li>
      <li>
        <BTN/>
      </li>
    </ul>
    <hr>
    <ul class="row">
      <li>
        ProMember
      </li>
      <li>
        <ul>
          <li>Unlimited Storage</li>
          <li>Unlimited Accounts</li>
          <li>Unlimited Connections</li>
        </ul>
      </li>
      <li>
        <ul>
          <li v-if="type==='yearly'">708$</li>
          <li v-else>70$</li>
          <li v-if="type==='yearly'">$59 per month</li>
          <li v-else></li>
          <li v-if="type==='yearly'">billed yearly</li>
          <li v-else>billed monthly</li>
        </ul>
      </li>
      <li>
        <BTN/>
      </li>
    </ul>

  </div>
</template>

<script>

import BTN from '@/components/Btn'

export default {
  data: () => ({
    type: 'yearly',
  }),
  components: {
    BTN,
  }
}

</script>

<style scoped>
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 0;
}

.row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 0;
}

.row li {
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0px;
  text-align: left;
}
.items{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 50px;
  padding-bottom: 50px;
}

.items h2{
  font-size: 48px;
  font-style: normal;
  font-weight: 700;
  line-height: 56px;
  letter-spacing: -0.8275861740112305px;
  text-align: left;
  color: #1D293F;
}

.btn-change{
  display: inline-flex;
  overflow: hidden;
  border: 2px solid #FFD166;
  border-radius: 10px;

}

button{
  background: #FFFFFF;
  border: none;
  outline: none;
  padding: 10px;
  height: 55px;
  width: 175px;
  font-size: 16px;
  font-weight: 500;
  letter-spacing: 0px;
  text-align: center;
  border-radius: 10px;
  cursor: pointer;
  color: #1D293F;
  /*border-radius: 10px 0px 0px 10px;*/
}

.active{
  background: #FFD166;
  border: 2px solid #FFD166;
  border-radius: 0;
}
</style>