<template>
<div>
    <div class="d-flex align-center mt-7 justify-space-between"> <h4 class="text-h6 white--text  ml-12" >HollyWood Movies</h4> <div class="d-flex align-center mr-10 purple--text text--lighten-3"><p class="mt-4 mr-2">More</p><v-icon class="purple--text text--lighten-3">mdi-greater-than</v-icon></div></div>
    <v-row class="ml-12 mt-3">
        <v-flex v-for="(pic,index) in movies" :key="index">
            <v-card  flat class=" ml-1 my-2" width="200">
                <v-img :src="pic.src" height="300"></v-img>
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
                src:"https://upload.wikimedia.org/wikipedia/en/2/2b/F9_film_poster.jpg"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/a/a7/Venom_Let_There_Be_Carnage_poster.jpg/220px-Venom_Let_There_Be_Carnage_poster.jpg"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/c/c6/Jungle_Cruise_-_theatrical_poster.png/220px-Jungle_Cruise_-_theatrical_poster.png"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/1/1c/Free_Guy_2021_Poster.jpg/220px-Free_Guy_2021_Poster.jpg"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/6/63/Godzilla_vs._Kong.png/220px-Godzilla_vs._Kong.png"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/8/8e/Dune_%282021_film%29.jpg/220px-Dune_%282021_film%29.jpg"
            }
        ]
    }
}
}
</script>