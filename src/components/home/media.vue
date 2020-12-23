<template>
  <v-container
    id="subscribe"
    tag="section"
    class="no-pd"
  >
    <base-card
     
      class="pa-0"
    >
      <v-container class="no-pd">
        <v-row class="justify-center mb-2">
            
              <v-img
              :aspect-ratio="16/9"
              :src="require('@/assets/media3.png')"
              class="grey lighten-2"
              max-height="400px"
              max-width="793px"
        >
      
        </v-img>

          
           
     
        </v-row>
        <v-row class="justify-start">
          
          
          <div
                class="ma-0"
                style="height: 48px; width: 35%; background-color: #6D4C41; text-align: center; color: white; padding: 4px;"
              

            
              >
              <h2>อีก 9 วัน</h2>
                
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
    padding-top: 0;
    padding-left: 1;
    padding-right: 1;
  }


</style>
