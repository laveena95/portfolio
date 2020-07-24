<template>
    <v-layout row align-center justify-center style="background-color:#f7f9fa;" class="ma-1" >
        <v-col cols="12" md="9">
            <v-card class="mt-6" flat align="center" justify="center" style="background-color:#f7f9fa;">
                <v-card-title primary-title class="layout justify-center"><h2>Contact</h2></v-card-title>
                    <v-card-content>
                        <p class="body-1">Interested in hiring me for your project or just want to say hi? You can fill in the contact form below or send me an email to <a href="" class="teal--text">simon.doe@yourwebsite.com</a></p>
                        <p class="body-1">Want to get connected? Follow me on the social channels below.</p>
                        
                        <v-list class="text-center" width="300" style="background-color:#f7f9fa;;">
                            <v-list-item class="mx-auto">
                                <div class="mx-auto mt-4" v-for="item in items" :key="item.id" style="background-color:#f7f9fa;">
                                    <v-btn class="mx-auto" x-small elevation="0" fab no outline>
                                        <v-icon color="teal" >{{ item.icon }}</v-icon>
                                    </v-btn>
                                </div>
                            </v-list-item>
                        </v-list>
                    </v-card-content>
            </v-card>
        </v-col>
    </v-layout>
</template>

<script>
export default {
    data: () => {
        return {
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
          icon: 'fab fa-instagram'
        },
        {
          id: '5',
          icon: 'fab fa-stack-overflow'
        },
        {
          id: '6',
          icon: 'fab fa-medium'
        },
        {
          id: '7',
          icon: 'fab fa-codepen'
        }
      ],
        }
    }

}
</script>

<style scoped>
a {
    text-decoration: none ;
}
</style>