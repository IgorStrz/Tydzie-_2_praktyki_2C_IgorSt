<template>
  <header>
    <h1>Witaj na stronie składającej się z paru bloków</h1>
  </header>
  <div class="LP">
    <h3>To jest lewy pasek</h3>
  </div>
  <div class="content">
    <img src="@/assets/meme.jpg" alt="This is FINE">
  </div>
  <div class="PP">
    <h3>To jest prawy pasek</h3>
  </div>
  <footer>
    <h2>Dziękuję za odwiedzenie mojej strony</h2>
  </footer>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  }
}
</script>
<style>
header {
  width: 100%;
  height: 100px;
  background-color: #A7E5AC;
}
.LP {
  width: 100px;
  height: 500px;
  background-color: #6096E6;
  float: left;
}
.content {
  width: 1320px;
  height: 500px;
  text-align: center;
  background-color: #E66C60;
  float: left;
}
.PP {
  width: 100px;
  height: 500px;
  background-color: #E6CE60;
  float: left;
}
footer {
  width: 100%;
  height: 100px;
  background-color: #EF2EF2;
  clear: both;
}
h1 {
  text-align: center;
  font-style: italic;
}
img {
  width: 400px;
  height: 500px;
}
h2 {
  text-align: center;
  font-style: arial;
  font-size: 30px;
}
h3 {
  text-align: center;
  font-style: arial;
}
</style>
