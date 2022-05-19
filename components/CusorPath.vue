<template>

<div >
  <v-main class="mt-1">
<v-carousel 
    cycle
    height="500"
    hide-delimiter-background
    show-arrows-on-hover
    id="cur"
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
      width="1200"
      class="ma-auto"
    >
      <v-btn  id="btn"><v-icon>mdi-play</v-icon>  Watch</v-btn>
    </v-carousel-item>
  </v-carousel>
  
  </v-main>
  <CardShow />
  <HorrorMovies/>
  <HollyWood />
  <FooterPage  />
  
  </div>

</template>

<script>
import CardShow from "./CardShow.vue"
import HorrorMovies from "./HorrorMovies.vue"
import FooterPage from "./FooterPage.vue"
import HollyWood from "./HollyWood.vue"

export default {
  components:{
    CardShow,
    HorrorMovies,
    FooterPage,
    HollyWood
  },
    data () {
      return {
        items: [
          {
            src: 'https://wallpaperaccess.com/full/7067663.jpg',
          },
          {
            src: '	https://images.ottplay.com/images/image-via-twitter-71.jpg',
          },
          {
            src: 'https://akamaividz2.zee5.com/image/upload/w_1420,h_569,c_scale,f_webp,q_auto:eco/resources/0-6-127/cover/1170x658withlogo809c4a89a8f14191881fc8f640492e96.jpg',
          },
          {
            src: 'https://www.koimoi.com/wp-content/new-galleries/2022/04/yash-sanjay-dutt-starrer-kgf-chapter-2-gets-a-5-star-rating-001.jpg',
          },
        ],
       
      }
    },
  }
</script>

<style>
#cur{
  margin:250 0;
}
#btn{
  position:relative;
  top:400px;
  left:30px;
  background-color:black;
  opacity: 0.6;
  border:1px solid white;
  color:white;
}
#btn:hover{
  background:white;
  color:black;
}
</style>