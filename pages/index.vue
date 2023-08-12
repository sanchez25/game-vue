<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
        <v-card-actions
          class="justify-center"
        >
          <v-btn
            class="pa-8"
            nuxt
            to="/game"
          >
            Play
          </v-btn>
          <v-btn
            class="pa-8"
            nuxt
            to="/"
          >
            Exit
          </v-btn>
        </v-card-actions>
    </v-col>
  </v-row>
</template>

<script>
  export default {
    name: 'IndexPage'
  }
</script>

<style>
</style>
