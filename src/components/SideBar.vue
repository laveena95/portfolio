<template>
  <div>
    <v-navigation-drawer
      app
      overflow
      color="teal"
       v-model="primaryDrawer.model"
      :clipped="primaryDrawer.clipped"
      :floating="primaryDrawer.floating"
      :mini-variant="primaryDrawer.mini"
      :permanent="primaryDrawer.type === 'permanent'"
      :temporary="primaryDrawer.type === 'temporary'"
    
    >
      <v-toolbar class="hidden-sm-and-up" color="teal" flat>
      <div class="hidden-sm-and-up">
        <v-menu offset-y>
          <template v-slot:activator="{ on }">
               <v-app-bar-nav-icon v-on="on"  
               v-if="primaryDrawer.type !== 'permanent'"
              @click.stop="primaryDrawer.model = !primaryDrawer.model"
              color="white"
              class="ml-n2 " large></v-app-bar-nav-icon>
          </template>
        </v-menu>
      </div>
      <h2 class="text-center white--text ">John Doe</h2>
    </v-toolbar>
      
      <v-list  >
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
        <v-divider class="mt-6" color=""></v-divider>
      </v-list>
      <v-list align-center v-for="menu in menues" :key="menu.id"> 
        <v-list-item :to="menu.route" color="teal" class="red--text">
          <v-list-item-icon>
            <v-icon small color="white" class="ml-4">{{ menu.icon}}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title class="white--text body-2">{{ menu.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list>
        <div class="text-center" >
          <v-btn rounded color="teal darken-3" dark>
            <v-icon small class="ma-2">fa fa-paper-plane</v-icon>
            Hire Me</v-btn>
        </div>
      </v-list>
      <v-divider class="mt-6"></v-divider>
      <v-container>
        <div class="text-center white--text">
          <h4> <v-icon color="white">brightness_medium</v-icon>
          Dark Mode</h4>
          <v-btn small center rounded outlined color="grey" class="ma-2" size="50">
            <v-switch
            v-model="$vuetify.theme.dark" inset
            outlined color="grey" large
          ></v-switch>
          </v-btn>
        </div>
      </v-container>
    </v-navigation-drawer>
   
    <v-toolbar class="hidden-sm-and-up" color="teal">
      <div class="hidden-sm-and-up">
        <v-menu offset-y>
          <template v-slot:activator="{ on }">
               <v-app-bar-nav-icon v-on="on"  
               v-if="primaryDrawer.type !== 'permanent'"
              @click.stop="primaryDrawer.model = !primaryDrawer.model"
              color="white"
              class="ml-n2 " large></v-app-bar-nav-icon>
          </template>
        </v-menu>
      </div>
      <h2 class="text-center white--text ">John Doe</h2>
    </v-toolbar>
  </div>
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
          route: '/'
        },
         {
          id: '2',
          icon: 'important_devices',
          title: 'Portfolio',
          route: '/portfolio'
        },
         {
          id: '3',
          icon: 'business_center',
          title: 'Services & Pricing',
          route: '/services'
        },
         {
          id: '4',
          icon: 'description',
          title: 'Resume',
          route: '/resume'
        },
         {
          id: '5',
          icon: 'pages',
          title: 'Blog',
          route: '/blog'
        },
         {
          id: '6',
          icon: 'move_to_inbox',
          title: 'Contact',
          route: '/contact'
        },
      ]
    }),
  }
</script>

<style scoped>

</style>