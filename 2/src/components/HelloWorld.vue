<template>
  <div class="przycisk">
    <button @click="handleClick">{{ i + 1 }}</button>
    <p>Liczba: {{ licz }}</p>
  </div>
</template>
<script>
export default {
  name: 'HelloWorld',
  props: {
    i: Number, 
    licz: Number 
  },
  methods: {
    handleClick() {
      this.$emit('dziala');
    }
  }
};
</script>
<style>
button {
  background-color: #00F00A;
  padding: 10px 20px;
  font-size: 10px;
  border: 10px solid #F0EC00;
  float: left;
}
p {
  color: #FFFFFF;
}
</style>
