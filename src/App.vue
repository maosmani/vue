<template>
  <v-app class="grey lighten-4">
     <NavBar/>
    <v-main>
      <HelloWorld/>

    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import NavBar from './components/NavBar.vue'

export default {
  name: 'App',

  components: {
    HelloWorld,
    NavBar,
  },

  data: () => ({
    //
  }),
}
</script>
