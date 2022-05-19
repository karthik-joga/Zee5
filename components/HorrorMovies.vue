<template>
<div>
    <h3 class="white--text ml-10">Horror Movies</h3>
    <v-row class="ml-12 mt-3">
        <v-flex v-for="(get,index) in images" :key="index">
        <v-card flat class=" ml-1 my-2" width="200">
            <v-img :src="get.src" height="300"></v-img>
        </v-card>

        </v-flex>
    </v-row>
</div>


</template>

<script>
export default{
    data(){
        return{
        images:[
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/0/06/Bhoot_Film_Poster.jpg/220px-Bhoot_Film_Poster.jpg"
            },
           {
                src:"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTn-Bj-3RuoYUd_TlUbD7168-ajZwXaDlrsFw&usqp=CAU"
            },
            {
                src:"https://upload.wikimedia.org/wikipedia/en/thumb/8/8d/Raju_Gari_Gadhi_3.jpg/220px-Raju_Gari_Gadhi_3.jpg"
            },
            {
                src:"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQOhg1tgwQSMmyym6ODpkl0YuTthvnWEqXyfQ&usqp=CAU"
            },
            {
                src:"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQsiYNo71MQMywyWHJ5HHVRuiSW-D5Ksztzrg&usqp=CAU"
            },
            {
                src:"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSP4ntTivOI5U-5DpJZ0k9E90rhFx7Rs1kx9w&usqp=CAU"
            },
            
        ]
    }
}
}
</script>