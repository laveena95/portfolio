<template>
<v-app id="sandbox">
    <v-navigation-drawer
      v-model="primaryDrawer.model"
      :clipped="primaryDrawer.clipped"
      :floating="primaryDrawer.floating"
      :mini-variant="primaryDrawer.mini"
      app
      overflow
      class="teal darken-1"
    >
      <h2 class="text-center white--text mt-6">John Doe</h2>
      <v-list>
      <v-list-item-avatar class="mt-6 ml-10" size="150">
          <img src="../assets/img/avatar.jpg" alt="">
      </v-list-item-avatar>
      <v-list-item>
        <p class="text-center white--text mt-4" style="font-size: 13px">Hi, my name is John Doe and I'm a senior software engineer. Welcome to my personal website!</p>
      </v-list-item>
      <v-list-item>
        <div class="text-center mt-4" v-for="item in items" :key="item.id">
          <v-btn class="mx-auto ml-2" fab x-small color="white">
            <v-icon color="teal">{{ item.icon }}</v-icon>
          </v-btn>
        </div>
      </v-list-item>
      <v-divider class="mt-6" dark></v-divider>
      </v-list>
      <v-list align-center v-for="menu in menues" :key="menu.id"> 
        <v-list-item>
          <v-list-item-icon>
            <v-icon small color="white">{{ menu.icon}}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title class="white--text">{{ menu.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list>
        <div class="text-center">
          <v-btn rounded color="teal darken-4" dark>
            <v-icon>near_me</v-icon>
            Hire Me</v-btn>
        </div>
      </v-list>
      <v-divider class="mt-6"></v-divider>

      <v-switch
        v-model="$vuetify.theme.dark"
        primary
        label="Dark"
      ></v-switch>
    </v-navigation-drawer>

    <v-main>
      <v-container fluid>
        <v-row
          align="center"
          justify="center"
        >         
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      primaryDrawer: {
        model: null,
      },
      items: [
        {
          id: '1',
          icon: 'fab fa-twitter'
        },
        {
          id: '2',
          icon: 'fab fa-linkedin-in'
        },
        {
          id: '3',
          icon: 'fab fa-github-alt'
        },
        {
          id: '4',
          icon: 'fab fa-stack-overflow'
        },
        {
          id: '5',
          icon: 'fab fa-codepen'
        }
      ],
      menues: [
        {
          id: '1',
          icon: 'fa fa-user',
          title: 'About Me',
        },
         {
          id: '2',
          icon: 'important_devices',
          title: 'Portfolio',
        },
         {
          id: '3',
          icon: 'business_center',
          title: 'Services & Pricing',
        },
         {
          id: '4',
          icon: 'description',
          title: 'Resume',
        },
         {
          id: '5',
          icon: 'pages',
          title: 'Blog',
        },
         {
          id: '6',
          icon: 'move_to_inbox',
          title: 'Contact',
        },
      ]
    }),
  }
</script>