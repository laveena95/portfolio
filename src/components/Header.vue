<template>
  <nav>
    <div class="ma-12 pa-12">
      <template>
        <v-container>
          <v-navigation-drawer permanent expand-on-hover dark class="fill-height">
            <v-list>
              <v-list-item link>
                <v-list-item-content>
                  <v-list-item-title class="title">Sandra Adams</v-list-item-title>
                  <v-list-item-subtitle>sandra_a88@gmail.com</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-list>

            <v-divider></v-divider>

            <v-list nav dense >
              <v-list-item link>
                <v-list-item-icon>
                  <v-icon>mdi-home</v-icon>
                </v-list-item-icon>
                <v-list-item-title>Home</v-list-item-title>
              </v-list-item>
              <v-list-item link>
                <v-list-item-icon>
                  <v-icon>mdi-pencil</v-icon>
                </v-list-item-icon>
                <v-list-item-title>About me</v-list-item-title>
              </v-list-item>
              <v-list-item link>
                <v-list-item-icon>
                  <v-icon>mdi-apple-airplay</v-icon>
                </v-list-item-icon>
                <v-list-item-title>My Skills</v-list-item-title>
              </v-list-item>
              <v-list-item link>
                <v-list-item-icon>
                  <v-icon>mdi-trophy</v-icon>
                </v-list-item-icon>
                <v-list-item-title>My Achievements</v-list-item-title>
              </v-list-item>
              <v-list-item link>
                <v-list-item-icon>
                  <v-icon>mdi-monitor-dashboard</v-icon>
                </v-list-item-icon>
                <v-list-item-title>My Projects</v-list-item-title>
              </v-list-item>
              <v-list-item link>
                <v-list-item-icon>
                  <v-icon>mdi-phone</v-icon>
                </v-list-item-icon>
                <v-list-item-title>Contact Me</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-navigation-drawer>
        </v-container>
      </template>
    </div>
  </nav>
</template>


<script>
  export default {
    name: 'Header',
  }
</script>