<template>
  <div class="container">
    <div class="items">
      <h2 class="w-50">Choose the right  plan for your finity</h2>
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

 <div class="row d-flex flex-column ">
   <hr>

   <ul class="row-item">
     <li class="plan-name">
       Starter
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
         <li v-if="type === 'yearly'" class="bigPriceBtn">228$</li>
         <li v-else class="bigPriceBtn">30$</li>
         <li v-if="type === 'yearly'" >$19 per month</li>
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
   <ul class="row-item">
     <li class="plan-name">
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
         <li v-if="type === 'yearly'" class="bigPriceBtn">468$</li>
         <li v-else class="bigPriceBtn">50$</li>
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
   <ul class="row-item">
     <li class="plan-name">
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
         <li v-if="type==='yearly'" class="bigPriceBtn">708$</li>
         <li v-else class="bigPriceBtn">70$</li>
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

  </div>
</template>

<script>

import BTN from '@/components/main/BTN'

export default {
  data: () => ({
    type: 'yearly',
  }),
  components: {
    BTN,
  }
}

</script>

<style lang="scss" scoped>
.bigPriceBtn{
  font-size: 58px !important;
  font-style: normal;
  font-weight: 500 !important;
  line-height: 64px !important;
  letter-spacing: -1px;
  color: #1D293F !important;
}

.row-item{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 40px 0;
}

.row-item li {
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 40px;
  letter-spacing: 0px;
}
.items{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 200px;
  padding-bottom: 50px;
}

.items h2{
  font-size: 48px;
  font-style: normal;
  font-weight: 700;
  line-height: 56px;
  letter-spacing: -0.8275861740112305px;
  color: #1D293F;
}

.btn-change{
  display: inline-flex;
  overflow: hidden;
  border: 2px solid #FFD166;
  border-radius: 10px;

}

button{
  border: 2px solid #FFD166;
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

@media screen and (max-width: 550px){
  .items{
    h2{
      font-size: 20px !important;
      line-height: 25px !important;
    }

    button{
      width: 140px;
      height: 40px;
    }
  }
}
@media screen and (max-width: 768px){
 .row{
   flex-direction: column;
   text-align: center;
 }

  .items {
    padding-top: 50px !important;
      h2{
        font-size: 27px;
        font-style: normal;
        font-weight: 700;
        line-height: 40px;
        letter-spacing: -0.827586174px;
        color: #1D293F;
      }
  }
  .row-item{
    flex-direction: column;
  }
}

@media screen and (max-width: 1000px){
    .items{
      flex-direction: column;
      align-items: center;
    }

  .plan-name{
    font-size: 45px !important;
    font-style: normal;
    font-weight: 700 !important;
    line-height: 64px !important;
    letter-spacing: -1px;
    color: #1D293F !important;
  }


}
</style>