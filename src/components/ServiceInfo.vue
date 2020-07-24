<template>
    <v-layout row align-center justify-center style="background-color:#f7f9fa;" >
        <v-col cols="12" md="9">
            <v-card class="mt-6 " width="" height="" flat align="center" justify="center" style="background-color:#f7f9fa;">
                <v-card-title primary-title class="layout justify-center"><h2>Services & Pricing</h2></v-card-title>
                    <v-card-text>
                        <p class="body-1">I have 10+ years of development experience building software for the web and mobile devices. You can take a look at my <a href="/portfolio" class="teal--text">project portfolio</a> and <a href="/resume" class="teal--text">online resume</a>to find out more about my skills and experiences.</p>         
                        <p class="body-1">I'm currently taking on freelance software development work. You're welcome to contact me for a custom quote for your project. I also offer development service packages with fixed pricing.</p>
                      </v-card-text>
                      <v-card-action>
                        <v-btn color="teal" dark align-center to="/contact"> <v-icon>near_me</v-icon><v-spacer></v-spacer> Hire me</v-btn>
                      </v-card-action>
            </v-card>
        </v-col>
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