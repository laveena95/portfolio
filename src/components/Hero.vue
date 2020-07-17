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
                  <h1 class="mb-5 ">Testimonials</h1>
                </v-list-item>
            </v-list>
          </v-col>
        </v-row>
      </v-col>
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
            width="300"
            
            @click="toggle" outlined=""
            >
            <v-card shaped="" elevation="10" style="background-color:teal;width:40px;height:40px;" class="">
                <v-icon dark small left class="ml-3 mt-2">fas fa-quote-left</v-icon>
            </v-card>
            <v-card-text class="">
                {{ text }}
            </v-card-text>
            
            <v-avatar size="70" class="ml-4">
                <v-img class="elevation-6" :src="item.src"></v-img>
            </v-avatar>
            <v-list-tile-content class="text-center">
                <v-list-tile-text class="ma-4 teal--text text-center">{{ item.name }}
                </v-list-tile-text>
                <div style="background-color:red; float:right;width:300px;"></div>
                
            </v-list-tile-content>
            
            </v-card>
            </v-col>
        </v-row>
        </v-slide-item>
        </v-slide-group>
    </v-container>
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
            src: require('../assets/img/avatar.jpg'),
            name: 'James Lee',
            place: 'Product Manager, Amazon',
          },
           {
            id: '2',
            src: require('../assets/img/avatar.jpg'),
            name: 'Olivia White',
            place: '',
          },
           {
            id: '3',
            src: require('../assets/img/avatar.jpg'),
            name: 'Samuel Reyes',
            place: '',
          },
           {
            id: '4',
            src: require('../assets/img/avatar.jpg'),
            name: 'Brandon James',
            place: '',
          },
           {
            id: '5',
            src: require('../assets/img/avatar.jpg'),
            name: 'Kate Sanders',
            place: '',
          },
           {
            id: '6',
            src: require('../assets/img/avatar.jpg'),
            name: 'Simon Doe',
            place: '',
          },
      ]
    }),
  }
</script>
<style>

</style>