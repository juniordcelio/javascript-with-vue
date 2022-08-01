<template>
  <v-app dark>
    <header>
      <v-row>
        <v-col>
          <v-btn to="/">index</v-btn>
        </v-col>  
        <v-col>
          <v-btn to="/calculadoraIMC">calculadora imc</v-btn>
        </v-col>
      </v-row>
    </header>
    <hr>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      fixed: false,
    }
  }
}
</script>

<style scoped>
header {
  background-color: white;
  height: 50px;
}
</style>
