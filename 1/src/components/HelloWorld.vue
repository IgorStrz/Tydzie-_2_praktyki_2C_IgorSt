<template>
  <div class="galeria">
    <h1>Galeria zdjęć</h1>
    <div class="XD">
      <div v-for="(zdj, i) in zdj" :key="i" class="NG">
        <p>{{ zdj.title }}</p>
        <img :src="zdj.url" :alt="zdj.title" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      zdj: [
        { url: require('@/assets/Doge.jpg'), title: "Doge" },
        {url: require('@/assets/BDoge.jpg'), title: "Bread doge" },
        { url: require('@/assets/SDoge.jpg'), title: "Sad doge" },
        { url: require('@/assets/GDoge.jpg'), title: "Giga chad doge" },
      ],
    };
  },
};
</script>
<style>
.galeria{
  text-align: center;
  background-color: #A6A6A6;
}
.NG{
  border: 5px solid #E80C4C;
  overflow: hidden;
  border-radius: 10px;
}
.XD{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 10px;
}
img{
  width: 100%;
  height: auto;
}
p{
  padding: 15px;
  background-color: #A6A6A6;
}
</style>