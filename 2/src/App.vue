<template>
  <div id="app">
    <div class="pudelko">
      <HelloWorld v-for="(liczba, klucz) in liczba2" 
        :key="klucz" 
        :klucz="klucz"
        :liczba="liczba"
        @dziala="increment(klucz)" />
    </div>
  </div>
</template>
<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      liczba2: Array(20).fill(0)
    };
  },
  methods: {
    increment(klucz) {
      this.liczba2[klucz]++;
    }
  }
};
</script>
<style>
body {
  background-color: #4307ED;
}
</style>
