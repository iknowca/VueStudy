<template>

  <v-container>
      <div>
          <router-link to="/">Home</router-link>|
          <router-link to="/about">about</router-link>|
          <router-link to="/html-test">htmltest</router-link>|
          <router-link to="/vue-data-binding-page">vue-data-binding-page</router-link>|
      </div>
  </v-container>

</template>

<script>
  import HelloWorld from '../components/HelloWorld'

  export default {
    name: 'Home',

    components: {
      HelloWorld,
    },
  }
</script>
