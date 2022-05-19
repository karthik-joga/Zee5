<template>
  <div>
      <v-app-bar app color="#0f0617" height="90"  class="d-flex ma-auto justify-space-between">
          <v-app-bar-title  >
               <v-img src="../../public/ZEE5_logo.svg" max-height="50" max-width="47"></v-img>
             
          </v-app-bar-title>
           <div class="white--text body-2 ma-6">Home</div>
              <div class="white--text body-2 ma-4">Tv show</div>
              <div class="white--text body-2 ma-4">Movies</div>
              <div class="white--text body-2 ma-4">Web series</div>
              <div class="white--text body-2 ma-4">News</div>
              <div class="ma-5" ><v-icon color="white">mdi-apps</v-icon> </div>
           <v-spacer ></v-spacer>

            <div class="rounded d-flex" color="white" id="search" height="20" width="70">
              <v-icon color="white" class="pa-2">mdi-magnify</v-icon>
              <input type="text"  id="text"  placeholder="search for Movies,Shows,Channels etc.">
            <v-icon  color="white" class="pa-2">mdi-microphone-outline</v-icon>
            
            </div>
            <v-hover>
            <div> <v-btn
                  v-show="!hidden"
                  color="black"
                  fab
                  dark
                  small
                  bottom
                  left
                  class="text-subtitle-1 ml-5"
                >
                  A
                </v-btn>
                <v-btn
                  v-show="!hidden"
                  color="black"
                  fab
                  dark
                  small
                  bottom
                  left
                  class="text-subtitle-1 ml-5"
                >
                  <v-icon>mdi-account</v-icon>
                </v-btn>
                 <v-btn
                  v-show="!hidden"
                  color="black"
                  fab
                  dark
                  small
                  bottom
                  left
                  class="text-subtitle-1 ml-5"
                >
                  <v-icon>mdi-menu</v-icon>
                </v-btn>
                </div>
          </v-hover>
      </v-app-bar>
 <CursorPath />
  </div>
</template>
<script>
import CursorPath from "./CusorPath.vue"
export default{
components:{
  CursorPath
}
}
</script>

<style>
#search{
  border:1px solid rgb(99, 99, 99);
  border-radius:2;
  height:35px;
  margin-left:285px;
  padding:5px
}
#text{
  width:225px;
}
#text::placeholder{
  font-size:small;
}
#text:focus{
  height:28px;
  outline:none;
  border:none;
  color:white
}
</style>