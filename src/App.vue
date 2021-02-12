<template>
  <div id="app">
    <RadioButton v-for="(animal, index) in animals" :key="index" :animal=animal></RadioButton>
  </div>
</template>

<script>
import RadioButton from './components/RadioButton'

export default {
  name: 'App',
  components: {
    RadioButton
  },
  data() {
    return {
      animals: [
        {id: '1', name: 'Cat'},
        {id: '2', name: 'Dog'}
      ]
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
