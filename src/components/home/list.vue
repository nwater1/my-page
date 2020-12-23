<template>
  <base-card class="custom-color">
  
    <v-img
      :src="require('@/assets/list.png')"
      class="mar-10"
      max-height="7076px"
      max-width="2625px"
      
    >
      
    </v-img>
  </base-card>
</template>

<script>
  export default {
    name: 'HomeBanner',
  }
</script>

<style scoped>
  .mar-10 {
    margin-left: 10px;
    margin-right: 10px;
  }
</style>

<style scoped>

  .custom-color {
  
        background-color: black;
 
}
</style>
