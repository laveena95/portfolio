<template>
    <v-col class="col-12 col-md-12">
      <v-container>
         <v-sheet elevation="0">
        <v-tabs
          v-model="tab"
          color="teal lighten-2"
          centered
          next-icon="mdi-arrow-right-bold-box-outline"
          prev-icon="mdi-arrow-left-bold-box-outline"
          show-arrows
        >
          <v-tab v-for="item in items" :key="item.tab">{{ item.tab }}</v-tab>
        </v-tabs>

        <v-tabs-items v-model="tab">
          <v-tab-item v-for="item in items" :key="item.tab">
            <v-row class="pt-16" no-gutters> 
              <v-col
                v-for="(content, index) in item.contents"
                :key="index"
                cols="12"
                md="6"
                class="px-5 py-4"
              >
                <v-hover>
                  <template v-slot:default="{ hover }">
                    <v-card elevation="0" outlined >
                      <v-row no-gutters>
                        <v-col class="col-4">
                          <v-img :src="content.src" height="100%"></v-img>
                        </v-col>
                        <v-col class="col-8 px-4 pt-3">
                          <p
                            class="dark text-h6 font-weight-bold text-decoration-underline"
                          >{{content.title}}</p>
                          <p
                            class="font-weight-light text-darken-1 mb-2 text-subtitle-2"
                          >{{content.text}}</p>

                          <p class="caption">Client:Google</p>
                          <v-fade-transition>
                            <v-overlay v-if="hover" absolute color="#2f435c">
                              <v-btn dark large class color="#2f435c">
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
          </v-tab-item>
        </v-tabs-items>
         </v-sheet>
      </v-container>
      
    </v-col>
</template>

<script>
export default {
  data() {
    return {
      tab: null,
      overlay: false,
      items: [
        {
          tab: "All",
          contents: [
            {
            id: '1',
            src: require('../assets/img/p1.jpg'),
            title:'Project Headline',
            text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
            client: 'Google',
        },
        {
            id: '2',
            src: require('../assets/img/p2.jpg'),
            title:'Project Headline',
            text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
            client: 'Dropbox',
        },
        {
            id: '3',
            src: require('../assets/img/p3.jpg'),
            title:'Project Headline',
            text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
            client: 'Google',
        },
        {
            id: '4',
            src: require('../assets/img/p4.jpg'),
            title:'Project Headline',
            text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
            client: 'Uber',
        },
            {
              id: '5',
              src: require('../assets/img/w3.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Salesforce',
            },
            {
              id: '6',
              src: require('../assets/img/w2.png'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Startup Hub',
            },
            {
              id: '7',
              src: require('../assets/img/m4.png'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Lyft',
            },
            {
              id: '8',
              src: require('../assets/img/f1.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Uber',
            }
          ]
        },
        {
          tab: "Web app",
          contents: [
            {
              src: require('../assets/img/w1.png'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
                client: 'Salesforce',
            },
            {
              src: require('../assets/img/w2.png'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
                client: 'Startup Hub',
            },
            {
              src: require('../assets/img/w3.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
                client: 'Lyft',
            }
          ]
        },
        {
          tab: "moblieApp",
          contents: [
            {
              src: require('../assets/img/m1.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
                client: 'Google',
            },
            {
              src: require('../assets/img/m2.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
                client: 'Dropbox',
                },
            {
              src: require('../assets/img/m3.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Starup Hub',
            },
            {
              src: require('../assets/img/m4.png'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Lyft',
            }
          ]
        },
        {
          tab: "Frond End",
          contents: [
            {
              src: require('../assets/img/f1.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Salesforce',
            },

            {
              src: require('../assets/img/f2.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Lyft',
            }
          ]
        },
        {
          tab: "Back End",
          contents: [
            {
              src: require('../assets/img/bk1.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Starup Hub',
            },
            {
              src: require('../assets/img/bk2.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Uber',
            },
            {
              src: require('../assets/img/bk3.jpg'),
              title: "Project Heading",
              text:
                "Project intro goes here. In the intro it's a good idea to answer a potential client's need/problem so it's more likelyto land your next project or job.",
              client: 'Lyft',
            }
          ]
        }
      ]
    };
  }
};
</script>