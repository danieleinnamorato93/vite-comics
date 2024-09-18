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
<div class="loadBtn"><a href="#"><button>Load More</button></a></div>


</main>
</template>

<style lang="scss" scoped>
main {
  position: relative;

  background-color: black;
  text-align: center;
 
  .jumbotron{
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    min-height: 300px;
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
  }}
  .loadBtn button {
  background-color: #0282F9;
  height: 35px;
  width: 140px;
  margin-bottom: 10px;
  border: none;
  color: white;
  font-weight: bold;
  font-size: 15px;

  }

}




</style>