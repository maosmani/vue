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
     
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-title>Foo</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Bar</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Fizz</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Buzz</v-list-item-title>
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
      drawer: false
    }
  }

}
</script>
