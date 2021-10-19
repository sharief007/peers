<template>
  <v-app>
    <v-row no-gutters>
      <v-col sm="4">
        <AppBar/>
        <Tabs/>
      </v-col>
      <v-col sm="8">
        <Nuxt/>
      </v-col>
    </v-row>
  </v-app>
</template>

<script>
import AppBar from "@/components/AppBar";
import Tabs from "@/components/Tabs";

export default {
  components: {
    AppBar,
    Tabs
  },
  data () {
    return {
      
    }
  }
}
</script>
