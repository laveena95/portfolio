<template>
    <v-app>
        <v-content transition="slide-x-transition">
            <Header/>
            <router-view></router-view>
        </v-content>
        <router-view></router-view>
    </v-app>
</template>


<script>

import Header from './components/Header';


export default {
  name: 'App',

  components: {
    Header,
  },

  data: () => ({
    //
  }),
};
</script>
