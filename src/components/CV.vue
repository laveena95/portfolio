<template>
  <v-container>
      <v-card elevation="18" flat class="ma-8">
          <div class="ma-4">
            <v-row>
                <v-col cols="9">
                    <v-card class="" flat height="50">
                        <v-card-title class="font-weight-bold teal--text h1"><h1>J O H N  D O E</h1></v-card-title>
                        <v-card-subtitle class="subtitle-1 mt-1">Senior Software Engineer</v-card-subtitle>
                    </v-card>
                </v-col>
                <v-col cols="3">
                <v-card flat="">
                    <v-list>
                        <div  v-for="item in items" :key="item.id" style="height:22px;border-left: 1px solid silver;" class="">
                        <v-list-item>
                            <v-icon small color="black" class="mb-4">{{ item.icon }}</v-icon>
                            <p class="caption ml-4 "> {{ item.text}} </p>
                        </v-list-item>
                        </div>
                    </v-list>
                </v-card>
                </v-col>
                <v-row class="mx-2">
                    <v-col cols="12" class="">
                            <v-divider class="" color="silver"></v-divider>
                    </v-col>
                </v-row>
            </v-row>
            <v-row class="">
                <v-col cols="2">
                    <v-avatar size="125" class="">
                        <img src="../assets/img/avatar.jpg" alt="">
                    </v-avatar>
                </v-col>
                <v-col cols="10">
                    <v-card flat height="80">
                        <v-card-text>
                            <p>
                                Summarise your career here. You can make a PDF version of your resume using our free Sketch template here. Donec quam felis, ultricies nec, pellentesque eu. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Maecenas nec odio et ante tincidunt tempus. Donec vitae sapien ut libero venenatis faucibus. Nullam quis ante. Etiam sit amet orci eget eros faucibus tincidunt. Duis leo. Sed fringilla mauris sit amet nibh.
                            </p>
                        </v-card-text>
                    </v-card>
                </v-col>
                <v-row class="mx-2">
                    <v-col cols="12" class="">
                        <v-divider class="mt-6" color="silver"></v-divider>
                    </v-col>
                </v-row>
            </v-row>
            <v-row>
                <v-col cols="9">
                    <div>
                        <div style="border-left: 5px solid teal" class="mt-n1 ml-4">
                            <h3 class="teal--text ml-3 "> WORK EXPERIENCES</h3>
                        </div>
                        <div>
                            <v-card flat>
                                <v-card-text >
                                    <v-row> 
                                        <h3 class="ml-3 black--text">Senior Software Engineer</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Google | 2019 - Present</p>
                                    </v-row>
                                    <p>
                                        Role description goes here ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Donec pede justo, fringilla vel. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis.
                                    </p>
                                    <v-list dense class="mt-n8">
                                        <v-list-item class="ml-4">
                                            <v-list-item-avatar size="5" color="black"></v-list-item-avatar>
                                            <v-list-item class="caption ml-n5"> Lorem ipsum dolor sit amet, consectetuer.</v-list-item>
                                        </v-list-item>
                                        <v-list-item class="ml-4">
                                            <v-list-item-avatar size="5" color="black" class="mt-n8"></v-list-item-avatar>
                                            <v-list-item class="caption ml-n5 mt-n10"> Aenean commodo ligula eget dolor.</v-list-item>
                                        </v-list-item>
                                        <v-list-item class="ml-4">
                                            <v-list-item-avatar size="5" color="black" class="mt-n15"></v-list-item-avatar>
                                            <v-list-item class="caption ml-n5 mt-n16"> Etiam ultricies nisi vel augue.</v-list-item>
                                        </v-list-item>
                                    </v-list>
                                </v-card-text>
                                <v-card-text class="mt-n12">
                                    <v-row> 
                                        <h3 class="ml-3 black--text" >Lead Software Developer</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Apple | 2016 - 2019</p>
                                    </v-row>
                                    <p>
                                        Role description goes here ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Donec pede justo, fringilla vel.
                                    </p>
                                    <v-list dense class="mt-n8">
                                        <v-list-item class="ml-4">
                                            <v-list-item-avatar size="5" color="black"></v-list-item-avatar>
                                            <v-list-item class="caption ml-n5">Lorem ipsum dolor sit amet, consectetuer.</v-list-item>
                                        </v-list-item>
                                        <v-list-item class="ml-4">
                                            <v-list-item-avatar size="5" color="black" class="mt-n8"></v-list-item-avatar>
                                            <v-list-item class="caption ml-n5 mt-n10">Aenean commodo ligula eget dolor.</v-list-item>
                                        </v-list-item>
                                    </v-list>
                                </v-card-text>
                                <v-card-text class="mt-n12">
                                    <v-row> 
                                        <h3 class="ml-3 black--text" >Senior Software Developer</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Dropbox | 2014 - 2016</p>
                                    </v-row>
                                    <p>
                                        Role description goes here ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
                                    </p>
                                </v-card-text>
                                <v-card-text class="mt-n8">
                                    <v-row> 
                                        <h3 class="ml-3 black--text" >Senior Developer</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Uber | 2013 - 2014</p>
                                    </v-row>
                                    <p>
                                        Role description goes here ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus.
                                    </p>  
                                </v-card-text>
                                <v-card-text class="mt-n8">
                                    <v-row> 
                                        <h3 class="ml-3 black--text" >Backend Developer</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Amazon | 2014 - 2016</p>
                                    </v-row>
                                    <p>
                                        Role description goes here ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
                                    </p>
                                </v-card-text>
                                <v-card-text class="mt-n8">
                                    <v-row> 
                                        <h3 class="ml-3 black--text" >Frontend Developer</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Startup | 2013 - 2014</p>
                                    </v-row>
                                    <p>
                                        Role description goes here ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus.
                                    </p>
                                </v-card-text>
                            </v-card>
                        </div>
                        <div style="border-left: 5px solid teal" class="mt-n1 ml-4">
                            <h3 class="teal--text ml-3"> PROJECTS</h3>
                        </div>
                        <div>
                            <v-card flat>
                                <v-card-text class="">
                                    <v-row> 
                                        <h3 class="ml-3 black--text" >Project Lorem Ipsum</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Startup | 2013 - 2014</p>
                                    </v-row>
                                    <p>
                                        You can use this section for your side projects. You can provide a project link here as well. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
                                    </p>
                                </v-card-text>
                                <v-card-text class="mt-n8">
                                    <v-row> 
                                        <h3 class="ml-3 black--text" >Project Sed Fringilla</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Open Source</p>
                                    </v-row>
                                    <p>
                                       You can use this section for your side projects. Cras dapibus. Vivamus elementum semper nisi. Aenean vulputate eleifend tellus. Aenean leo ligula, porttitor eu, consequat vitae, eleifend ac, enim. 
                                    </p>  
                                </v-card-text>
                                       <v-card-text class="mt-n8">
                                    <v-row> 
                                        <h3 class="ml-3 black--text" >Project Praesent</h3>
                                        <v-spacer> </v-spacer>
                                        <p class="caption">Open Source</p>
                                    </v-row>
                                    <p>
                                        You can use this section for your side projects. Cras dapibus. Vivamus elementum semper nisi. Aenean vulputate eleifend tellus. Aenean leo ligula, porttitor eu, consequat vitae, eleifend ac, enim
                                    </p>
                                </v-card-text>
                            </v-card>
                        </div>
                    </div>
                </v-col>
                <v-col cols="3">
                    <div style="border-left: 1px solid silver;" >
                        <div style="border-left: 5px solid teal;" class="mt-n1 ml-4">
                            <h3 class="teal--text ml-3"> SKILLS</h3>
                        </div>
                        <div>
                            <v-card flat class="" width="400">
                                <v-card-text>
                                    <h3 class="black--text" >Technical</h3>
                                    <v-list>
                                        <v-list-item class="body-2 ml-n3">JavaScript/Angular/React/Vue</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt-n4">Python/Ruby/PHP</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt-n4">Node.js/ASP.NET</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt-n4">PostgreSQL/MySQL.</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt-n4">Object-oriented design</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt-n2">Design and implement database structures</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt">Lead and deliver complex software systems</v-list-item>
                                    </v-list>
                                </v-card-text>
                                 <v-card-text>
                                    <h3 class="black--text" >Professional</h3>
                                    <v-list>
                                        <v-list-item class="body-2 ml-n3">Effective communication</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt-n4">Team player</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt-n4">Strong problem solver</v-list-item>
                                        <v-list-item class="body-2 ml-n3 mt-n4">Good time management</v-list-item>
                                    </v-list>
                                </v-card-text>
                            </v-card>
                        </div>
                        <div style="border-left: 5px solid teal;" class="mt-n1 ml-4">
                            <h3 class="teal--text ml-3"> EDUCATION</h3>
                        </div>
                        <div>
                            <v-card flat class="">
                                <v-card-text>
                                   <h4 class="black--text" >MSc in Computer Science</h4>
                                   <p class="body-2">University College London <br> 2010 - 2011</p>
                                
                                   <h4 class="black--text" >BSc Maths and Physics</h4>
                                   <p class="body-2">Imperial College London <br> 2007 - 2010</p>
                                </v-card-text>
                            </v-card>
                        </div>
                        <div style="border-left: 5px solid teal;" class="mt-n1 ml-4">
                            <h3 class="teal--text ml-3"> AWARDS</h3>
                        </div>
                        <div>
                            <v-card flat class="">
                                <v-card-text>
                                   <h4 class="black--text" >Award Lorem Ipsum</h4>
                                   <p class="body-2">Microsoft lorem ipsum <br>(2019)</p>
                                
                                   <h4 class="black--text" >Award Donec Sodales</h4>
                                   <p class="body-2">Imperial College London <br> Oracle Aenean (2017)</p>
                                </v-card-text>
                            </v-card>
                        </div>
                        <div style="border-left: 5px solid teal;" class="mt-n1 ml-4">
                            <h3 class="teal--text ml-3"> LANGUAGES</h3>
                        </div>
                        <div>
                            <v-card flat class="">
                                <v-card-text>
                                   <v-list>
                                       <v-list-item class="body-2 ml-n3 mt-n5">Tamil (Native)</v-list-item>
                                       <v-list-item class="body-2 ml-n3 mt-n5">English (Professional)</v-list-item>
                                   </v-list>
                                </v-card-text>
                            </v-card>
                        </div>
                        <div style="border-left: 5px solid teal;" class="mt-n1 ml-4">
                            <h3 class="teal--text ml-3"> INTERESTS</h3>
                        </div>
                        <div>
                            <v-card flat class="">
                                <v-card-text>
                                   <v-list>
                                       <v-list-item class="body-2 ml-n3 mt-n5">Climbing</v-list-item>
                                       <v-list-item class="body-2 ml-n3 mt-n5">Snowboarding</v-list-item>
                                          <v-list-item class="body-2 ml-n3 mt-n5">Photography</v-list-item>
                                       <v-list-item class="body-2 ml-n3 mt-n5">Travelling</v-list-item>
                                   </v-list>
                                </v-card-text>
                            </v-card>
                        </div>
                    </div>
                </v-col>
            </v-row>
            <v-row class="mx-2">
                    <v-col cols="12" class="">
                        <v-divider class="mt-2" color="silver"></v-divider>
                    </v-col>
                </v-row>
            <v-row>
                <v-col cols="2.5"></v-col>
                <v-col cols="2">
                    <v-row>
                        <v-icon  fab class="mb-4"> fab fa-github-square </v-icon>
                        <a href="" class="caption black--text ml-1">github.com/username</a>
                    </v-row>
                </v-col>
                <v-col cols="2.5">
                    <v-row>
                        <v-icon  fab class="mb-4 ml-4"> fab fa-linkedin </v-icon>
                        <a href="" class="caption black--text ml-1">linkedin.com/in/username</a>
                    </v-row>
                </v-col>
                <v-col cols="2" >
                    <v-row>
                        <v-icon  fab class="mb-4"> fab fa-twitter-square </v-icon>
                        <a href="" class="caption black--text ml-1">@twittername</a>
                    </v-row>
                </v-col>
                <v-col cols="2.5"></v-col>
            </v-row>
        </div>
      </v-card>
  </v-container>
</template>

<script>
export default {
    data: () => {
        return {
            items: [
                {
                    id: '1',
                    icon : 'fa fa-phone-square',
                    text: '0123 4567 890',
                    path: '',
                },
                {
                    id: '2',
                    icon : 'fa fa-envelope-square',
                    text: 'john.doe@yourwebsite.com',
                    path: '',
                },
                {
                    id: '3',
                    icon : 'language',
                    text: 'www.yourwebsite.com',
                    path: '',
                },
                {
                    id: '4',
                    icon : 'location_on',
                    text: 'Newyork',
                    path: '',
                },
            ],
        }
    }

}
</script>

<style scoped>
a{
    text-decoration: none;
}


.fab:hover{
    color: teal;
}
</style>