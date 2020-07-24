<template>
    <v-layout row align-center justify-center style="background-color:#f7f9fa;" >
            <v-col cols="12" md="9">
                <v-card class="mt-6" width="" height="" flat align="center" justify="center" style="background-color:#f7f9fa;">
                    <v-card-title primary-title class="layout justify-center"><h2>Portfolio</h2></v-card-title>
                        <v-card-text align-center>
                            <p class="body-1">Welcome to my online portfolio. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. I'm taking on freelance work at the moment. Want some help building your software?</p>
                           </v-card-text>
                           <v-card-action>
                                <v-btn color="teal" dark align-center to="/contact"> <v-icon small class="ma-2"> fa fa-paper-plane</v-icon><v-spacer></v-spacer> Hire me</v-btn>
                           </v-card-action>
                </v-card>
            </v-col>
    </v-layout>
</template>

<script>
export default {

}
</script>

<style>

</style>