<script>
import ComicsList from "./ComicsList.vue";

export default {
  data() {
    return {
      
    }
  },
  components:{
    ComicsList
  } 
}
</script>

<template>
<main>
  <div class="jumbotron"></div>
<button>CURRENT SERIES</button>
<ComicsList />
</main>
</template>

<style lang="scss" scoped>
main {
  position: relative;
  min-height: 500px;
  background-color: black;
 
  .jumbotron{
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    min-height: 300px;
  }
}
button {
  background-color: #0282F9;
  padding: 20px;
  border: none;
  color: white;
  position: absolute;
  top: 265px;
  left: 170px;
}

</style>