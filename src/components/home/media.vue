<template>
  <v-container
    id="subscribe"
    tag="section"
    class="no-pd"
  >
  <base-subheading style="color: white; text-align: center;">สวดมนต์ข้ามปี ออนไลน์</base-subheading>
    <base-card
     
      class="pa-0"
    >
      <v-container class="no-pd" style="background-color: blue">
        <v-row class="justify-center mb-2" style="background-color: blue">
            
              <v-img
              
              :src="require('@/assets/media-live.png')"
              class="grey lighten-2"
              max-height="800px"
              max-width="793px"
        >
      
        </v-img>

          
           
     
        </v-row>
        <v-row class="justify-start">
          
          
          <div
                class="ma-0"
                style="height: 40px; width: 35%; background-color: blue; text-align: center; color: white; padding: 4px;"
              

            
              >
              <h2>share:</h2>
                
          </div>
        </v-row>
      </v-container>
    </base-card>
  </v-container>
</template>

<script>
  export default {
    name: 'media',
  }
</script>

<style scoped>
  .no-pd {
    padding-top: 5;
    padding-left: 1;
    padding-right: 1;
  }


</style>
