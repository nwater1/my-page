<template>
  <v-container
    id="blog"
    tag="section"
  >
    <base-subheading style="color: white; margin-top: 15px;">ธรรมะประจำวัน</base-subheading>

    <p style="color: white;">
      ช่วงปีใหม่นี้ แจกฟรี บทสวดมนต์เสริมสิริมงคล อ่านธรรมะดีๆทุกๆวัน
    </p>
      <vue-horizontal-list :items="items" :options="options">
      <template v-slot:default="{ item }">
        <v-card max-width="400px">
          <div class="image-container">
            <img :src="item.image" aspect-ratio="1.7" cover />
          </div>

          <div class="subtitle">
            
          </div>
          <v-card-actions class="justify-center" style="margin-top: 0px;">
            <v-btn color="#6D4C41" width="25%">
              <p style="color: white; margin-bottom: 0">อ่านต่อ</p>
            </v-btn>
          </v-card-actions>
        </v-card>
      </template>
    </vue-horizontal-list>
  </v-container>
</template>

<script>
import VueHorizontalList from "vue-horizontal-list";
  export default {
    name: 'HomeAbout',
    components: {
      VueHorizontalList,
  },
  data() {
    return {
      items: [
        {
          title: "Sed non ante non cras amet",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas non sagittis leo. Vestibulum sit amet metus nec neque dignissim dapibus.",
          image: "https://my-page.s3-ap-southeast-1.amazonaws.com/vdo2.png",
        },
        {
          title: "Curabitur sit amet nunc",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec id mollis erat. Aliquam erat volutpat. Nunc erat lacus, rhoncus nec.",
          image: "https://my-page.s3-ap-southeast-1.amazonaws.com/text2.png",
        },
        {
          title: "Proin pharetra, ante metus",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi ac diam ac ex efficitur posuere. Pellentesque cursus pellentesque risus, non.",
          image: "https://picsum.photos/id/1039/600/600",
        },
        {
          title: "Cras pharetra non enim a",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi malesuada varius nibh, a malesuada nisi feugiat eget. Aenean convallis semper.",
          image: "https://picsum.photos/id/1042/600/600",
        },
        {
          title: "Proin vulputate, augue eu accumsan",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas fringilla tempor libero sit amet mollis. Praesent quis leo erat. Integer.",
          image: "https://picsum.photos/id/1044/600/600",
        },
        {
          title: "Maecenas feugiat magna sapien in",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam sit amet fringilla ante. Quisque at ipsum non lacus consequat dictum.",
          image: "https://picsum.photos/id/1057/600/600",
        },
        {
          title: "Donec commodo sed enim at",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc eu condimentum risus. Praesent dignissim, neque nec pharetra vestibulum, libero odio.",
          image: "https://picsum.photos/id/1063/600/600",
        },
        {
          title: "In bibendum urna et turpis",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse vitae ante volutpat leo vulputate volutpat et sed ex. Vivamus eu.",
          image: "https://picsum.photos/id/1076/600/600",
        },
        {
          title: "Phasellus iaculis dignissim erat at",
          content:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla mattis quam scelerisque, eleifend purus gravida, scelerisque orci. Ut et turpis.",
          image: "https://picsum.photos/id/1083/600/600",
        },
      ],
      options: {
        responsive: [
          { end: 576, size: 1 },
          { start: 576, end: 768, size: 2 },
          { start: 768, end: 992, size: 3 },
          { size: 4 },
        ],
      },
    };
  },
  }
</script>

<style scoped>

.subtitle {
  margin-top: 8px;
  margin-bottom: 6px;
  display: flex;
  justify-content: space-between;
  font-size: 14px;
  font-weight: 500;
}
.image-container {
  border-radius: 3px;
  overflow: hidden;
  position: relative;
  width: 100%;
  padding-top: 125%;
}
img {
  object-fit: cover;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
}
</style>
