<template>
    <div>
        <v-text-field v-model="altura" type="number" outlined label="Altura"/>
        <v-text-field v-model="peso" type="number" outlined label="Peso"/>
        <v-btn @click="calcula">Calcular IMC</v-btn>
        <p>{{resultado}}</p>
    </div>
</template>

<script>
export default {
  name: 'calculadora-imc',
  data() {
    return {
      resultado: null,
      altura: null,
      peso: null,
    }
  },
  computed: {},
  methods: {
    calcula () {
        this.resultado = this.peso/(this.altura*this.altura)
    }
  }
}
</script>