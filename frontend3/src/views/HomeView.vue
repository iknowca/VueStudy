<template>
  <v-container>
    <div>
      <nav>
        <router-link to="/">Home</router-link>|
        <router-link to="/about">about</router-link>

      </nav>
    </div>
  </v-container>
</template>

<script>
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'HomeView',

  components: {
  },
});
</script>
