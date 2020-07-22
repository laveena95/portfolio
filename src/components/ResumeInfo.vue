<template>
    <v-layout row align-center justify-center style="background-color:#f7f9fa;" >
            <v-card class="mt-6" width="800" height="150" flat align="center" justify="center" style="background-color:#f7f9fa;">
                <v-card-title primary-title class="layout justify-center"><h2>Online Resume</h2></v-card-title>
                    <v-card-content>
                        <v-btn color="teal" dark align-center to="/"> <v-icon small class="ma-2"> fa fa-file-pdf </v-icon><v-spacer></v-spacer> Download pdf version</v-btn>
                    </v-card-content>
            </v-card>
    </v-layout>
</template>

<script>
export default {

}
</script>

<style scoped>
a {
    text-decoration: none ;
}
</style>