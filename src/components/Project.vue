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
                <h1 class="mb-5 ">Featured_Projects</h1>
            </v-list-item>
        </v-list>
        </v-col>
    </v-row>
    </v-col>
    <v-row>
        <v-col cols="12" md="6" v-for="item in items" :key="item.id">
            <v-hover>
                
          <v-card>
            <div class="d-flex flex-no-wrap justify-space-between">
              <div>
                <v-card-title
                  class="headline ma-3"
                  v-text="item.title"
                > <h5><hr>{{ item.title }}</h5></v-card-title>
                <div>
                    <v-card-text class="ma-3">{{ item.text }}</v-card-text>
                </div>
              </div>

              <v-avatar
                class="ma-3"
                height="200"
                width="700"
                left=""
                tile
              >
                <v-img :src="item.src"></v-img>
              </v-avatar>
            </div>
          </v-card>
            </v-hover>
        </v-col>
        <v-container class="text-md-center mb-10">
        <v-btn color="teal" dark align-center to="/portfolio"> <v-icon>mdi-arrow-right-bold-circle</v-icon><v-spacer></v-spacer> View Portfolio</v-btn>
      </v-container>
    </v-row>
  </v-container>
</template>

<script>
export default {
data: () =>({
    items: [
        {
            id: '1',
            src: require('../assets/img/avatar.jpg'),
            title:'Project Headline',
            text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
            client: 'Google',
        },
        {
            id: '2',
            src: require('../assets/img/avatar.jpg'),
            title:'Project Headline',
            text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
            client: 'Dropbox',
        },
        {
            id: '3',
            src: require('../assets/img/avatar.jpg'),
            title:'Project Headline',
            text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
            client: 'Google',
        },
        {
            id: '4',
            src: require('../assets/img/avatar.jpg'),
            title:'Project Headline',
            text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
            client: 'Uber',
        },
    ]
})
}
</script>

<style scoped>
a{
    text-decoration: none;

}
</style>