<template>
    <v-app>
        <v-content transition="slide-x-transition">
            <SideBar/>
            <router-view></router-view>
        </v-content>
        <router-view></router-view>
    </v-app>
</template>


<script>

import SideBar from './components/SideBar';


export default {
  name: 'App',

  components: {
    SideBar,
  },

  data: () => ({
    //
  }),
};
</script>
