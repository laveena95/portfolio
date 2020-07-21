<template>
    <v-layout row align-center justify-center style="background-color:;" >
            <v-card class="mt-6" width="600" height="" flat align="center" justify="center" style="background-color:;">
                <v-card-title primary-title class="layout justify-center"><h2>Get In Touch</h2></v-card-title>
                    <v-card-content>
                        <v-form>
                            <v-container>
                                <v-row >
                                    <v-col cols="12" sm="6" >
                                        <v-text-field
                                            label="Name"
                                            v-model="name"
                                            :rules="nameRules"
                                            single-line
                                            outlined
                                            color="teal lighten-2"
                                        ></v-text-field>
                                    </v-col>
                                    <v-col cols="12" sm="6">
                                        <v-text-field
                                            label="Email"
                                            v-model="email"
                                            :rules="emailRules"
                                            single-line
                                            outlined
                                            color="teal lighten-2"
                                        ></v-text-field>
                                    </v-col>
                                    <v-col class="d-flex" cols="12">
                                        <v-select
                                        :items="items"
                                        :rules="[v => !!v || 'Please select your service package!']"
                                        label="Select a service package you're interested in..."
                                        dense
                                        single-line
                                        outlined
                                        hint="Want to know what's included in each package? Check the Services & Pricing page."
                                        persistent-hint
                                        color="teal lighten-2"
                                        >
                                        </v-select>
                                    </v-col>
                                    <v-col cols="12">
                                          <v-textarea
                                            label="Enter your message"
                                            single-line
                                            outlined
                                            color="teal lighten-2"
                                            ></v-textarea>
                                    </v-col>
                                    <v-col cols="12">
                                         <v-btn block dark color="teal accent-4" type="submit">Send Now</v-btn>
                                    </v-col>
                                </v-row>
                            </v-container>
                        </v-form>
                    </v-card-content>
            </v-card>
    </v-layout>
</template>

<script>
  export default {
    data: () => ({
      valid: true,
      name: '',
      nameRules: [
        v => !!v || 'Name is required',
        v => (v && v.length <= 10) || 'Name must be less than 10 characters',
      ],
      email: '',
      emailRules: [
        v => !!v || 'E-mail is required',
        v => /.+@.+\..+/.test(v) || 'E-mail must be valid',
      ],
      select: null,
      items: [
        'Basic',
        'Standard',
        'Premium',
        'Not sure',
      ],
    }),
  }
</script>
<style scoped>

</style>