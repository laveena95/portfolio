<template>
 <v-container>
     <v-col cols="12" md="4">
        <v-row>
          <v-col cols="12" md="2">
            <v-card height="45px" width="5px" color="teal" class="ml-10">
            </v-card>
          </v-col>
          <v-col cols="12" md="10">
            <v-list two-line="" subheader="" class="nl-n8">
              <v-list-item>
                  <h1 class="mb-5 ">What I Do</h1>
                </v-list-item>
            </v-list>
          </v-col>
        </v-row>
      </v-col>
      <v-container>
        <p class="ml-10">I have more than 10 years' experience building software for clients all over the world. Below is a quick overview of my main technical skill sets and technologies I use. Want to find out more about my experience? Check out my <a href="/resume" class="teal--text">online resume</a> and <a href="/portfolio" class="teal--text">project portfolio</a>.</p>
      </v-container>
    <v-row>
      <v-col v-for="item in items" :key="item.id" class="d-flex child-flex" cols="12" md="3"> 
        <v-card flat>
          <v-list-item>
            <v-avatar v-for="image in item.src" tile v-bind:key="image" size="40" style="border-radius:0;">
                <v-img :src="image" ></v-img>
            </v-avatar>
            </v-list-item>
          <v-card-title><h5>{{ item.title }}</h5></v-card-title>
          <v-card-text><p>{{ text }}</p></v-card-text>
        </v-card>
      </v-col>
      <v-container class="text-md-center mb-10">
        <v-btn color="teal" dark align-center to="/services"> <v-icon>mdi-arrow-right-bold-circle</v-icon><v-spacer></v-spacer> Service & Pricing</v-btn>
      </v-container>
    </v-row>
 </v-container>
</template>

<script>
export default {
     name: 'Skill',
     data: () => {
       return{
         text:'List skills/technologies here. You can change the icon above to any of the 1500+ FontAwesome 5 free icons available. Aenean commodo ligula eget dolor.',
          items:[
         {
           id: '1',
           src: ['img/java.png'],
           title: 'Vanilla JavaScript',
         },
         {
           id: '2',
           src: ['img/Angular1.png','img/react.png','img/vue.png'],
           title: 'Angular, React & Vue',
         },
         {
           id: '3',
           src: ['img/nj.png'],
           title: 'Node.js',
         },
         {
           id: '4',
           src: ['img/python.png'],
           title: 'Python & Django',
         },
         {
           id: '5',
           src:['img/php.png'],
           title: 'PHP',
         },
         {
           id: '6',
           src: ['img/npm.png','img/Gulp.png','img/grunt.png'],
           title: 'npm, Gulp & Grunt',
         },
         {
           id: '7',
           src: ['img/html.png','img/CSS3.jpg'],
           title: 'HTML & CSS',
         },
         {
           id: '8',
           src: ['img/saaa.png','img/canvas.png'],
           title: 'Sass & LESS',
         },

       ]
       }}
      
}
</script>

<style scoped>
  a{
    text-decoration: none;
    color: teal;
  }
</style>