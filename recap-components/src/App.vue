<template>
  <h1>Ciaooo</h1>
</template>

<script>
import axios from 'axios'
export default {
  data() {
    return {

    }
  },
  methods: {
    getRandomCard() { 
      axios.get('https://api.magicthegathering.io/v1/cards?page=1&pageSize=1')
       .then(res => {
          console.log(res)
        })
    }
  },
  mounted() {
    this.getRandomCard()
  },
}
</script>

<style lang="scss"></style>
