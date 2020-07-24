<template>
  <v-container>
    <v-row align-center justify-center>
        <v-col cols="12" class="ml-8" xs="6">
        <div style="border-left:5px solid teal">
            <h1 class="ml-4">Latest Blog Posts</h1>
        </div>
        </v-col>
    </v-row>
    <v-container>
        <v-row class="ma-1">
            <v-col  v-for="item in items" :key="item.id" cols="12" md="4">
                <v-card  class="mx-auto" flat width="" height="550" color="#f7f9fa">
                    <v-img
                    :src="item.src"
                    aspect-ratio="1.5" 
                    ></v-img>
                    <div>
                        <v-card-title primary-title>
                            <h5 class=" mb-0"><u>{{ item.title }}</u></h5>
                        </v-card-title>
                        <v-card-text class="body-2"> {{ item.text }}</v-card-text>
                        <v-card-actions>
                        <p class="teal--text ml-2 body-2">Read More <v-icon small color="teal">trending_flat</v-icon></p>
                        </v-card-actions>
                        <v-card-text>{{ item.day }}</v-card-text>
                    </div>
                </v-card>
            </v-col>
        </v-row>
        <v-row class="mx-9">
            <v-col cols="12" sm="">
                <v-container class="text-md-center mb-10">
                <v-btn color="teal" dark align-center to="/blog"> <v-icon>mdi-arrow-right-bold-circle</v-icon><v-spacer></v-spacer> View blog</v-btn>
            </v-container>
            </v-col>
        </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
    data: () => ({
        items: [
            {
                id: '1',
                src: require('../assets/img/b1.jpg'),
                title: 'Top 3 JavaScript Frameworks',
                text: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient...',
                day:'Published 2 days ago',
            },
            {
                id: '2',
                src: require('../assets/img/b2.jpg'),
                title: 'About Remote Working',
                text: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient...',
                day:'Published a week ago',
            },
            {
                id: '3',
                src: require('../assets/img/b3.jpg'),
                title: 'A Guide to Becoming a Full-Stack Developer',
                text: 'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient...',
                day:'Published 3 weeks ago',
            }
        ]
    })
}
</script>

<style>

</style>