<template>
  <v-container > 
    <v-row align-center justify-center>
      <v-col cols="12" class="ml-8">
        <div style="border-left:5px solid teal">
          <h1 class="ml-4">Testimonial</h1>
        </div>
      </v-col>
    </v-row>
    <v-row>
      <v-container>
        <v-slide-group
        v-model="model"
        class="pa-4"
        center-active
        show-arrows
        >
        <v-slide-item
            v-for="n in 6"
            :key="n"
            v-slot:default="{ active, toggle }"
        >
        <v-row>
            <v-col  v-for="item in items" :key="item.id">
                <v-card
            class="m1-2"
            height="300"
            width="300" color="#f7f9fa"
            
            @click="toggle" outlined=""
            >
            <v-card shaped="" elevation="10" style="background-color:teal;width:40px;height:40px;" class="">
                <v-icon dark small left class="ml-3 mt-2">fas fa-quote-left</v-icon>
            </v-card>
            <v-card-text class="">
                {{ text }}
            </v-card-text>
            <v-row>
              <v-col>
                <v-avatar size="70" class="ml-4">
                <v-img class="elevation-6" :src="item.src"></v-img>
            </v-avatar>
              </v-col>
              <v-col>
                <v-list-tile-content class="caption">
               <p class="ml-n15 mt-4">{{ item.name }} <br> {{ item.place }} </p>
            </v-list-tile-content>
              </v-col>
            </v-row>
            </v-card>
            </v-col>
        </v-row>
        </v-slide-item>
        </v-slide-group>
    </v-container>
    </v-row>
    <v-divider class="mt-6"></v-divider>
    <v-row></v-row>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      model: null,

      text: "Simon is a brilliant software engineer! Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis.",

      items: [
          {
            id: '1',
            src: require('../assets/img/i1.jpg'),
            name: 'James Lee',
            place: 'Product Manager, Amazon',
          },
           {
            id: '2',
            src: require('../assets/img/i5.jpg'),
            name: 'Olivia White',
            place: 'Product Manager, Dropbox',
          },
           {
            id: '3',
            src: require('../assets/img/i2.jpg'),
            name: 'Samuel Reyes',
            place: 'CTO, StartupHub',
          },
           {
            id: '4',
            src: require('../assets/img/i3.jpg'),
            name: 'Brandon James',
            place: 'Project Manager, Google',
          },
           {
            id: '5',
            src: require('../assets/img/i6.png'),
            name: 'Kate Sanders',
            place: 'Project Manager, Uber',
          },
           {
            id: '6',
            src: require('../assets/img/i4.jpg'),
            name: 'Simon Doe',
            place: 'Project Manager, Google',
          },
      ]
    }),
  }
</script>
<style>

</style>