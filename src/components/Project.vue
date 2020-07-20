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
     <v-row class="pt-16" no-gutters> 
              <v-col
                v-for="item in items"
                :key="item.id"
                cols="12"
                md="6"
                class="px-5 py-4"
              >
                <v-hover>
                  <template v-slot:default="{ hover }">
                    <v-card elevation="0" outlined >
                      <v-row no-gutters>
                        <v-col class="col-4">
                          <v-img :src="item.src" height="100%"></v-img>
                        </v-col>
                        <v-col class="col-8 px-4 pt-3">
                          <p
                            class="dark text-h6 font-weight-bold text-decoration-underline text-decoration-color:grey"
                          >{{item.title}}</p>
                          <p
                            class="font-weight-light text-darken-1 mb-2 text-subtitle-2"
                          >{{item.text}}</p>

                          <p class="caption">Client : {{ item.client }}</p>
                          <v-fade-transition>
                            <v-overlay v-if="hover" absolute color="#2f435c">
                              <v-btn dark large class color="black">
                                <v-icon right dark class="mx-1">mdi-eye</v-icon>View Case Study
                              </v-btn>
                            </v-overlay>
                          </v-fade-transition>
                          
                        </v-col>
                      </v-row>
                    </v-card>
                  </template>
                </v-hover>
              </v-col>
            </v-row>
            <v-divider class="mt-6"></v-divider>
  </v-container>
</template>

<script>
export default {
data: () =>({
    items: [
        {
            id: '1',
            src: require('../assets/img/p1.jpg'),
            title:'Project Headline',
            text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
            client: 'Google',
        },
        {
            id: '2',
            src: require('../assets/img/p2.jpg'),
            title:'Project Headline',
            text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
            client: 'Dropbox',
        },
        {
            id: '3',
            src: require('../assets/img/p3.jpg'),
            title:'Project Headline',
            text:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
            client: 'Google',
        },
        {
            id: '4',
            src: require('../assets/img/p4.jpg'),
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
.v-card--reveal {
  align-items: center;
  bottom: 0;
  justify-content: center;
  opacity: .8;
  position: absolute;
  width: 100%;
}
</style>