<script>
import Header from "../src/components/Header.vue";
export default {
  components: {
    Header,
  },
};
</script>

<template>
  <div>
    <Header />
    <router-view class="container" />
  </div>
</template>

<style>
body {
  margin: 0px;
  box-sizing: border-box;
  font-family: "Avenir", sans-serif;
  color: #234;
}
ul {
  list-style: none;
  padding: 0px;
  margin: 0px;
}
a {
  font-weight: bold;
  text-decoration: none;
  color: #234;
}
a.router-link-active {
  color: #4b8;
}

.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}

.v-enter {
  opacity: 0;
  transform: translate3d(-20px, 0, 0);
}

.v-enter-active {
  transition: all 0.3s;
}

img {
  max-width: 100%;
}

.conteudo {
  display: grid;
  grid-template-columns: 1fr minmax(280px, 400px);
  grid-gap: 30px;
}

@media screen and (max-width: 700px) {
  .conteudo {
    display: block;
  }
}
</style>
