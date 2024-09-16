<script>
export default {
  data() {
    return {
      navLinks :[
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
<header>
<div class="logo"><img src="../assets/img/dc-logo.png" alt="header-logo"></div>
<ul>
<li v-for="navItem in navLinks">
 <a href="#">{{ navItem }}</a> 
</li>
</ul>
</header>
</template>

<style lang="scss" scoped>
header{
    background-color: white;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    .logo >img {
    height: 60px;
    width: auto;
    margin-top: 5px;
    margin-bottom: 20px;
  }
    ul {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  text-align: center;
  li {
    margin-right: 10px;
    font-size: 12px;
    font-weight: bold;
    color: #4A4C4C;
    a{
      color: inherit;
      &:hover {
    color: #0282F9;
    border-bottom: 2px solid #0282F9;

    }
    }
  
  }

}
}

</style>