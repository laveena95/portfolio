<template>
  <v-container style="background-color:#f7f9fa;" >
      <v-row class="" align-content="center">
        <v-col cols="12" md="9">
          <v-card width="" flat align-center>
          <v-container style="background-color:#f7f9fa;">
            <div class="d-flex flex-no-wrap justify-space-between text--justify">
              <div>
                <v-card-title
                  class="headline"
                ><h1>John Doe</h1></v-card-title>
                <v-card-subtitle class="mt-4" ><h2 style="font-weight:300;color:back;">Senior Software Engineer</h2></v-card-subtitle>
                <v-card-text><p>I'm a software engineer specialised in frontend and backend development for complex scalable web apps. I write about software development on <a href="/blog" class="teal--text">my blog</a>. Want to know how I may help your project? Check out my project <a href="/portfolio" class="teal--text">portfolio</a> and online <a href="/resume" class="teal--text">resume</a>.</p>
              </v-card-text>
              </div> 
            </div>
            <v-card-actions>
              <v-row>
                <v-col cols="12" md="3">
                  <v-btn color="teal" dark class="">
                  <v-icon small color="white mx-auto ml-2"> fas fa-arrow-circle-right</v-icon><v-sapcer> </v-sapcer>
                  View Portfolio</v-btn>
                </v-col>
                <v-col cols="12" md="3">
                  <v-btn color="black" dark class="">
                  <v-icon small color="white">description</v-icon><v-spacer> </v-spacer>
                  View Resume</v-btn>
                </v-col>
              </v-row>
              </v-card-actions>
          </v-container>
          </v-card>
        </v-col>
        <v-col cols="12" md="3" class="">
          <v-card flat>
             <v-avatar
                class=""
                size="275"
                tile
              >
                <img src="../assets/img/avatar.jpg" alt="" class="">
              </v-avatar>
          </v-card>
        </v-col>
      </v-row>
  </v-container>
</template>

<script>
export default {
    name: 'Info'
}
</script>

 <style scoped>
 a{
   text-decoration: none;
   color:turquoise;
   font-weight: 500;
 }
 </style>