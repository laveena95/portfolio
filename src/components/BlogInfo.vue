<template>
    <v-layout row align-center justify-center style="background-color:#f7f9fa;" >
        <v-col cols="12" md="8">
            <v-card class="mt-6" flat align="center" justify="center" style="background-color:#f7f9fa;">
                <v-card-title primary-title class="layout justify-center"><h2>A Blog About Software Development And Life</h2></v-card-title>
                    <v-card-content>
                        <p class="body-1">Welcome to my blog. Subscribe and get my latest blog post in your inbox.</p>
                    </v-card-content>
                    <v-container>
                        <v-row align-center justify-center>
                            <v-col cols="12" md="2"></v-col>
                            <v-col cols="12" sm="6" md="6">
                                <v-text-field
                                    label="Enter email"
                                    v-model="email"
                                    :rules="emailRules"
                                    single-line
                                    outlined
                                    dense=""
                                    color="teal lighten-2"
                                ></v-text-field>
                                </v-col>
                                <v-col cols="12" md="2"><v-btn color="teal" dark block class=""> subscribe</v-btn></v-col> 
                        </v-row>
                    </v-container>
            </v-card>
        </v-col>
    </v-layout>
</template>

<script>
export default {

}
</script>

<style scoped>
 .v-text-field{
      width: '200px';
}
</style>