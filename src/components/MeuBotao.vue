<template>
  <div>
    <button @click="incremento">{{ texto }}</button>
  </div>
</template>
<script>
export default {
  data () {
    return {
      contador: 0
    }
  },
  computed: {
    vezes () {
      return this.contador === 1 ? 'vez' : 'vezes'
    },
    texto () {
      return `Clicado ${this.contador} ${this.vezes}`
    }
  },
  methods: {
    incremento () {
      this.contador += 1
    }
  }
}
</script>
