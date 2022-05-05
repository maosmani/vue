<template>
  <nav>
    <v-toolbar flat app>
       <v-app-bar-nav-icon  @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title class="text-uppercase grey--text"> 
        Democracy
      </v-toolbar-title>
     
      <v-btn flat color="grey">
        <span>Sign Out </span>
        <v-icon right>mdi-exit-to-app</v-icon>
      </v-btn>
    </v-toolbar>
    <v-navigation-drawer 
     app 
     v-model="drawer"
      absolute
      bottom
      temporary>

          <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6">
            Open Democracy
          </v-list-item-title>
          
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>
      <v-list>

        <v-list-item-group v-model="model">
        <v-list-item>
          <v-list-item-icon>
            <v-icon></v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title ></v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>

      </v-list>

    

    </v-navigation-drawer>
  </nav>
  
</template>

<script>

export default {
  data() {
    return {
      drawer: false,
        items: [
        ['mdi-email', 'Inbox'],
        ['mdi-account-supervisor-circle', 'Supervisors'],
        ['mdi-clock-start', 'Clock-in'],
      ],
        
    }
  }

}
</script>
