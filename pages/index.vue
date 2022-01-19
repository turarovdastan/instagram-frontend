<template>
  <v-card class="mx-auto" max-width="1000" tile>
      <v-img height="200" src="https://c.wallhere.com/photos/47/ad/nature_landscape_mountains_mist_Moon_starry_night_moonlight_dark-104501.jpg!d"></v-img>
      <v-row style="margin:2.5%;position:absolute; top: 130px">
        <v-list-item>
        <v-list-item-avatar size="100">
            <img
            elevation="24"
            src="@/assets/profile.jpg"
            alt="John"
            >
        </v-list-item-avatar>
        </v-list-item>
    </v-row>
     <v-card style="margin-top:60px;" class="col-12">
            <v-card-title>
            Turarov Dastan
            </v-card-title>

            <v-card-subtitle>
            Web developer
            </v-card-subtitle>
            <v-card-text>Все мы гении. Но если вы будете судить рыбу по её способности взбираться на дерево, она проживёт всю жизнь, считая себя дурой.</v-card-text>
            <v-row justify="space-around" class=" my-5">
                <v-btn icon>
                    <v-icon
                        color=" light"
                        >
                        mdi-phone
                    </v-icon> 
                </v-btn>
                 <v-btn icon>
                    <v-icon
                        color=" light"
                        >
                        mdi-gmail
                    </v-icon> 
                </v-btn>
                 <v-btn icon>
                    <v-icon
                        color=" light"
                        >
                        mdi-instagram
                    </v-icon> 
                </v-btn>
            </v-row>
    </v-card>

    <v-divider></v-divider>


    <v-card style="padding:10px 10px 30px 10px;">
    <div class="swiper">
    <!-- Additional required wrapper -->
    <div class="swiper-wrapper">
       <div class="swiper-slide">
          <img src="@/assets/s1.jpg" />
        </div>
        <div class="swiper-slide">
          <img src="@/assets/s2.jpg" />
        </div>
        <div class="swiper-slide">
          <img src="@/assets/s3.jpg" />
        </div>
        <div class="swiper-slide">
          <img src="@/assets/s4.jpg" />
        </div>
        <div class="swiper-slide">
          <img src="@/assets/s5.jpg" />
        </div>
        <div class="swiper-slide">
         <video src="@/assets/miyagi.mp4" controls></video>
       </div>
    </div>
    <!-- If we need pagination -->
    <div class="swiper-pagination"></div>
    </div>
     <v-card-text>Каждый живет, как хочет, и расплачивается за это сам.</v-card-text>
    </v-card>
  </v-card>
</template>



<script>
import Swiper from 'swiper/swiper-bundle.min.js'
import 'swiper/swiper-bundle.min.css'
export default {
    mounted(){
        const swiper = new Swiper('.swiper', {
            grabCursor: true,
            effect: "creative",
                creativeEffect: {
                prev: {
                    shadow: true,
                    translate: [0, 0, -400],
                },
                next: {
                    translate: ["100%", 0, 0],
                },
            },
            loop: true,

            // If we need pagination
            pagination: {
                el: '.swiper-pagination',
            },
        });
    }
}
</script>


<style scoped>
.swiper {
  width: 100%;
  height: 500px;
}

 img,video{
      width: 100%;
      height: 100%;
    }
</style>