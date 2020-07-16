<template>
  <v-container>
    <v-row
      align="center"
    >
    <v-col
        cols="12"
      >
        <v-card width="1000" flat align-center>
          <v-container >
            <div class="d-flex flex-no-wrap justify-space-between text--justify">
              <div>
                <v-card-title
                  class="headline"
                ><h1>John Doe</h1></v-card-title>

                <v-card-subtitle class="mt-4" ><h2 style="font-weight:300;color:back;">Senior Software Engineer</h2></v-card-subtitle>
                <v-card-text><p>I'm a software engineer specialised in frontend and backend development for complex scalable web apps. I write about software development on <a href="/blog">my blog</a>. Want to know how I may help your project? Check out my project <a href="/portfolio">portfolio</a> and online <a href="/resume">resume</a>.</p>
              </v-card-text>
              <v-card-actions>
                <v-btn color="teal" dark>
                  <v-icon small color="white mx-auto ml-2"> fas fa-arrow-circle-right</v-icon>
                  View Portfolio</v-btn>
                  <v-btn color="black" dark>
                  <v-icon small color="white">description</v-icon>
                  View Resume</v-btn>
              </v-card-actions>
                </div>
              <v-avatar
                class="ma-3"
                size="275"
                tile
              >
                <img src="../assets/img/avatar.jpg" alt="">
              </v-avatar>
            </div>  </v-container>
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