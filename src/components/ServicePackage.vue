<template>
    <v-layout row align-center justify-center  >
        <v-card class="mt-6" width="800" height="" flat align="center" justify="center">
            <v-card-title primary-title class="layout justify-center"><h2>Services Packages</h2></v-card-title>
                <v-simple-table dense table-border="1">
                    <template v-slot:default>
                    <thead>
                        <tr class="text-center teal--text mt-4" style="background-color:">
                        <th ></th>
                        <th ><h3>Basic</h3></th>
                        <th ><h3>Standard</h3></th>
                        <th ><h3>Premium</h3></th>
                        </tr>
                    </thead>
                    <tbody class="" >
                        <tr v-for="item in packages" :key="item.name">
                        <td class="text-left"><h5 class="mt-8">{{ item.name }}</h5> <br/> <p> {{ item.text }}</p> </td>
                        <td class="text-center">{{ item.basic }} <v-icon color="teal"> {{ item.icon1}}</v-icon> </td>
                        <td class="text-center">{{ item.standard }} <v-icon color="teal"> {{ item.icon2}}</v-icon></td>
                        <td class="text-center">{{ item.premium }} <v-icon color="teal"> {{ item.icon3}}</v-icon></td>
                        </tr>
                        <tr >
                            <td class="text-center ma-4">  </td>
                            <td > <v-btn color="teal" dark align-center class="text-center ma-4">book now</v-btn></td>
                            <td > <v-btn color="teal" dark align-center class="text-center ma-4">book now</v-btn></td>
                            <td > <v-btn color="teal" dark align-center class="text-center ma-4">get a quote</v-btn></td>
                        </tr>
                    </tbody>
                    </template>
                </v-simple-table>
        </v-card>
    </v-layout>
</template>

<script>
  export default {
    data () {
      return {
          
        packages: [
          {
            name: 'Package Price',
            basic: '$900',
            standard: '$2500',
            premium: '$5000+',
          },
           {
            name: 'Details',
            basic: 'A small app lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.',
            standard: 'An medium app lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.An medium app lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.',
            premium: 'A complex app lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.',
          },
          {
            name: 'Feature Lorem',
            text: "Optional feature description goes here. Lorem ipsum dolor sit amet, consectetuer adipiscing elit.",
            icon1:'mdi-check',
            icon2:'mdi-check',
            icon3:'mdi-check',
          },
          {
            name: 'Feature Ipsum',
            text: "Optional feature description goes here. Lorem ipsum dolor sit amet, consectetuer adipiscing elit.",
            icon1:'mdi-check',
            icon2:'mdi-check',
            icon3:'mdi-check',
          },
          {
            name: 'Feature Commodo',
            icon1:'mdi-check',
            icon2:'mdi-check',
            icon3:'mdi-check',
          },
          {
            name: 'Feature Consectetuer',
            basic: '_',
            icon2:'mdi-check',
            icon3:'mdi-check',
          },
          {
            name: 'Feature Aenean',
            basic: '_',
            standard: '_',
            icon3:'mdi-check',
          },
          {
            name: 'Feature Duis',
            basic: '_',
            standard: '_',
            icon3:'mdi-check',
          },
          {
            name: 'Revisions',
            basic: '1',
            standard: '2',
            premium: '5+',
          },
          {
            name: 'Delivery Time',
            basic: '7 days',
            standard: '14 days',
            premium: '2 - 3 month(s)',
          },
        ],
      }
    },
  }
</script>
