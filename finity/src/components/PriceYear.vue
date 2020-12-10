<template>
  <div>
    <div>
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

    <div v-if="type === 'yearly'">
      yearly
    </div>

    <div v-else>
      monthly
    </div>


  </div>
</template>

<script>
export default {
  data: () => ({
    type: 'yearly',
  }),
}
</script>