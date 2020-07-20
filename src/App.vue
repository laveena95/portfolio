<template>
    <v-app>
       <SideBar/>
        <v-content >
          <router-view></router-view>
        </v-content>
        <Footer/>
    </v-app>
</template>


<script>

import SideBar from './components/SideBar';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    SideBar,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>
