<template>
    <div>
      <v-footer color="deep-orange darken-3" padless :absolute="!fixed" align="center"  class="py-4 white--text" >
        <v-container>
          <!-- add footer content here -->
          <v-row>
              <v-col cols="12" sm="12" md="3" lg="3">
                <h3 class="mb-2">community</h3>
                <div v-for="(item, index) in data" :key="index">
                  <v-icon left size="25" class="mt-1">{{ item.icon }}</v-icon>
                  <span>{{ item.name }}</span>    
                </div>
              </v-col>
              <v-col cols="12" sm="12" md="3" lg="3">
                <h3 class="mb-2">Useful Links</h3>
                <div v-for="(item, index) in data" :key="index">
                  <span>{{ item.name }}</span>    
                </div>
              </v-col>
              <v-col cols="12" sm="12" md="3" lg="3">
                <h3 class="mb-2">Resources</h3>
                 <div v-for="(item, index) in data" :key="index">
                  <span>{{ item.name }}</span>    
                </div>
              </v-col>
              <v-col cols="12" sm="12" md="3" lg="3">
                <h3 class="mb-2">Others</h3>
                 <div v-for="(item, index) in data" :key="index">
                  <span>{{ item.name }}</span>    
                </div>
              </v-col>
          </v-row>
        </v-container>
      </v-footer>
      <div class="deep-orange darken-2 white--text">
        <v-row justify="space-between" no-gutters>
        <span class="ma-4">Developed By : Techminate</span>
        <span class="ma-4">Copyright © Techminate {{ new Date().getFullYear() }}</span>
        </v-row>
      </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      fixed: true,
      data:[
        {"title":"First", "icon":"mdi-state-machine", "name":"Lorem "},
        {"title":"Clean", "icon":"mdi-console", "name":" ipsum "},
        {"title":"Documentation", "icon":"mdi-file-document-multiple-outline", "name":"dolor"},
      ]
    }
  }
}
</script>

<style>

</style>