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
<div class="currentBtn"><a href="#"><button>CURRENT SERIES</button></a></div>
<ComicsList />

</main>
</template>

<style lang="scss" scoped>
main {
  position: relative;
  min-height: 700px;
  background-color: black;
 
  .jumbotron{
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    min-height: 300px;
  }
}
.currentBtn button {
  background-color: #0282F9;
  padding: 15px;
  border: none;
  color: white;
  font-weight: bold;
  font-size: 15px;
  position: absolute;
  top: 265px;
  left: 170px;
  &:hover{
    background-color: white;
    color:#0282F9;
  }

}


</style>