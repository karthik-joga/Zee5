<template>

<div class="mb-5" >
   <div class="d-flex align-center mt-7 justify-space-between"> <h4 class="text-h6 white--text  ml-12" >Exclusive Movies on ZEE5</h4> <div class="d-flex align-center mr-10 purple--text text--lighten-3"><p class="mt-4 mr-2">More</p><v-icon class="purple--text text--lighten-3">mdi-greater-than</v-icon></div></div>
 
<v-row class="ml-12 my-5">   
<v-flex  v-for="(person,index) in movies" :key="index">
<v-card flat class=" ml-1 mr-1" width="200">
 <v-img :src= "person.src" height="300" >
    </v-img>
</v-card>
</v-flex>
</v-row>
    </div>
</template>

<script>
export default{
data(){
    return{
        movies:[
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/d/d7/RRR_Poster.jpg/220px-RRR_Poster.jpg"
            },
              {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/d/d4/The_Kashmir_Files_poster.jpg/220px-The_Kashmir_Files_poster.jpg"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/7/75/Pushpa_-_The_Rise_%282021_film%29.jpg/220px-Pushpa_-_The_Rise_%282021_film%29.jpg"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/d/d0/K.G.F_Chapter_2.jpg/220px-K.G.F_Chapter_2.jpg"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/6/6b/Saaho_poster.jpg"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/8/89/Gangubai_Kathiawadi_film_poster.jpg/220px-Gangubai_Kathiawadi_film_poster.jpg"
            },
            
        ]
    }
}
}
</script>