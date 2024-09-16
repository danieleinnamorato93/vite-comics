<script>
export default {
  data() {
    return {
      navUtilities :[ "DC COMICS",
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ]
      
    }
  }
}
</script>

<template>
<section>
  <div class="links">
    <ul>
 <h4>DC COMICS</h4>
  <li v-for="link in navUtilities">
    <a href="#">{{ link }}</a>
  </li>
</ul>
<ul>
 <h4>SHOP</h4>
 <li v-for="link in navUtilities">
    <a href="#">{{ link }}</a>
  </li>
</ul>
<ul>
 <h4>SITES</h4>
 <li v-for="link in navUtilities">
    <a href="#">{{ link }}</a>
  </li>
 
</ul>

  </div>


<div class="logobg"><img src="../assets/img/dc-logo-bg.png" alt=""></div>
</section>
</template>

<style lang="scss" scoped>
section {
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  min-height: 300px;
  display: flex;
  justify-content:space-around;
  align-items: center;
  
  
}
ul {
text-align: start;
  margin: 0 20px;
}
ul h4 {
  color: white;

  margin-bottom: 15px;
}
a {
  color:grey;
  font-size: 10px;
  margin: 0;
  padding-top: 5px;
  &:hover {
    color: #0282F9;
  }
}
li {
  display: flex;
  align-items: flex-start;
}
.links{
  display: flex;
  justify-content: flex-start;
  text-align: left;
  flex-basis: 30%;
}
.logobg {
  flex-basis: 30%;
}
</style>