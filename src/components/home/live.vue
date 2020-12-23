<template>
  <base-card class="rounded-lg" color="#0D47A1" style="padding-top: 5px; text-align: center; padding-bottom: 10px;">

    <base-subheading style="color: white;">สวดมนต์ข้ามปี ออนไลน์</base-subheading>
    <v-img
      :src="require('@/assets/media-live.png')"
      class="mar-10"
      max-height="2427px"
      max-width="2260px"
      
    >
      
    </v-img>
    <v-row style="margin-left: 5px; margin-top: 15px" class="justify-center">
      <base-subheading style="color: white;">share:</base-subheading>
      <div style="margin-left: 0px;">
          <vue-goodshare-facebook
    page_url="https://www.facebook.com/dhamma1000000"
    title_social="Facebook"
    has_icon
    style="margin-left: 5px;"
  ></vue-goodshare-facebook>
  <vue-goodshare-line
    page_url="https://www.facebook.com/dhamma1000000"
    title_social="Line"
    has_icon
    style="margin-left: 10px;"
  ></vue-goodshare-line>
      </div>
      
  
    </v-row>


    
  </base-card>
</template>

<script>
 import VueGoodshareFacebook from "vue-goodshare/src/providers/Facebook.vue";
 import VueGoodshareLine from "vue-goodshare/src/providers/Line.vue";
  export default {
    name: 'HomeBanner',
    
      components: {
    VueGoodshareFacebook, 
    VueGoodshareLine
  }
    
  }
</script>

<style scoped>
  .mar-10 {
    margin-top: 20px;
    margin-left: 10px;
    margin-right: 10px;
    
  }
</style>

<style scoped>

  
</style>
