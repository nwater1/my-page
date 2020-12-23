<template>
  <v-container
    id="subscribe"
    tag="section"
  >
    <base-card
      color="rgba(203, 170, 92, 0.51)"
      class="pa-3"
    >
      <v-container>
        <v-row class="justify-center">
          <v-col
            cols="12"
            
            
          >
            <base-subheading class="mb-3" style="color: white; text-align: center;">
              ปี2564 ชะตาชีวิตของคุณจะเป็นอย่างไร อยู่ที่คุณกำหนดเอง
            </base-subheading>

            <p style="color: white; text-align: center;">
              สวดมนต์ข้ามปีออนไลน์ ผ่าน 99 วัด 99 สิ่งศักดิ์สิทธิ์ เพื่อเปลี่ยนชะตาชีวิต ในชั่วข้ามปี
            </p>
            <p style="color: white; text-align: center;">
              สวดมนต์พร้อมกันทั้งครอบครัว ได้ทุกที่ทุกมุมโลก
            </p>

            <v-row class="pa-2 justify-center">
              <v-responsive
                class="overflow-visible mr-2"
                max-width="400"
              >
                <v-text-field
                  hide-details
                  label="Your Email Address"
                  solo
                />
              </v-responsive>

              <v-btn
                :block="$vuetify.breakpoint.xsOnly"
                class="ma-0"
                color="secondary"
                style="height: 48px"
              >
                Subscribe
              </v-btn>
            </v-row>
          </v-col>

          
        </v-row>
      </v-container>
    </base-card>
  </v-container>
</template>

<script>
  export default {
    name: 'HomeSubscribe',
  }
</script>
