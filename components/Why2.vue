<template>
    <v-container>
        <v-row class="">
            <v-col cols="12" sm="12" md="6" lg="6">
                <div class="text-uppercase ml-5">
                    <p class="font-weight-medium text-h5 mt-10">We Create Result-Oriented Dynamic Applications</p>
                    <p class="mt-5">When building business web apps, one of the most common tasks is data entry, that is, lots of webforms bound to domain objects or POJOs, validated against sometimes complex logic and finally persisted in a database or perhaps over REST to a remote server.</p>
                </div>
                <div class="mt-10">
                    <div v-for="(item, index) in data" :key="index" class="d-flex my-6">
                        <div class="mr-3">
                            <v-icon left size="50" :color="item.color">{{ item.icon }}</v-icon>
                        </div>
                        <div>
                          <span>{{ item.title }}</span>
                          <p>{{ item.description }}</p>
                        </div>
                    </div>
                </div>     
            </v-col>
            <v-col cols="12" sm="12" md="6" lg="6">
                <div class="text-center mt-15">
                    <span class="">
                        <img class="mt-5" src="~/assets/why/why.png" quality="90" width="600" height="392" fit="fill" />
                    </span>
                </div>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
  metaInfo: {
    
  },
  data(){
    return{
      data:[
        {"title":"First Growing Proccess","color":"blue", "icon":"mdi-state-machine", "description":"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
        {"title":"Clean Code","color":"purple", "icon":"mdi-console", "description":"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
        {"title":"Well Documentation","color":"red", "icon":"mdi-file-document-multiple-outline", "description":"Lorem ipsum dolor sit amet consectetur adipisicing elit."},
      ]
    }
  }
}
</script>

<style scoped>

</style>
