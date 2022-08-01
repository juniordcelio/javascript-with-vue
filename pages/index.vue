<template>
  <div>
    <h1>{{ text }}</h1>
    <v-btn
      @click="mudaTexto()"
    >
      CLIQUE AQUI
    </v-btn>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      text: 'Olá mundo',
      cont: 0
    }
  },
  computed: {},
  methods: {
    mudaTexto() {
      this.text = 'clicou '+this.cont++
    }
  }
}
</script>

<style scoped>

</style>
