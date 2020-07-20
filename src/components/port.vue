<template>
  <v-tabs
          fixed-tabs
          v-model="tab"
        >
          <v-tabs-slider color="amber darken-3"></v-tabs-slider>
          <v-tab
            v-for="(item, index) in items"
            :class="{active: currentTab === index}"
            @click="currentTab = index"
            :key="item"
          >
            {{ item }}
          </v-tab>
        <v-tabs-items v-model="tab">
          <v-card flat>            
            <div v-show="currentTab === 0">
              <v-container fluid>
          <v-row>
            <v-col cols="12" md="6" v-for="item in items" :key="item.id">
                <v-hover>
                    <v-card slot-scope="{ hover }" class="mx-auto" flat color="" outlined="">
                        <div class="d-flex flex-no-wrap justify-space-between">
                        <div>
                            <v-card-text
                            class=" ma-3 "
                            style="text-decoration:underline;text-decoration-color:grey;"
                            > <h3 >{{ item.title }}</h3></v-card-text>
                            <div>
                                <v-card-text class="ma-3">{{ item.text }}</v-card-text> 
                                <v-card-text class="ml-3 monospace--text">Client : {{ item.client }}</v-card-text>
                            </div>
                        </div>

                        <v-avatar
                            class="ma-3"
                            height="250"
                            width="700"
                            tile
                        >
                            <v-img :src="item.src">
                            
                            </v-img>
                        </v-avatar>
                        
                        </div>
                        <v-expand-transition>
                            <div
                                v-if="hover"
                                class="d-flex transition grey darken-2 v-card--reveal display-3 white--text"
                                style="height: 100%;"
                            >
                                <v-btn dark color="black darken-4"><v-icon>mdi-eye</v-icon><v-spacer> </v-spacer> View Case Study</v-btn>
                            </div>
                        </v-expand-transition>
                    </v-card>
                </v-hover>
            </v-col>
          </v-row>
        </v-container>
              </div>
            <div v-show="currentTab === 1"><v-card-text>Tab1 content</v-card-text></div>
            <div v-show="currentTab === 2"><v-card-text>Tab2 content</v-card-text></div>
            <div v-show="currentTab === 3"><v-card-text>Tab3 content</v-card-text></div>
            <div v-show="currentTab === 4"><v-card-text>Tab4 content</v-card-text></div>
          </v-card>
        </v-tabs-items>
      
  </v-tabs>

</template>


<script>

export default {
   data () {
     return {
      currentTab: 0,
      tab: null,
      items: ['All', 'web app', 'mobile', 'backend', 'frontend'],
     }
  }}
  </script>
<style>

</style>