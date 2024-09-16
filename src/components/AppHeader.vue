<script>
export default {
  data() {
    return {
      navLinks :[
        "Characters",
        "Comics",
        "Movies",
        "Tv",
        "Games",
        "Collectibles",
        "Videos",
        "Fans",
        "News",
        "Shop",
    ]
    }
      
  }
}
</script>

<template>
<header>
<div class="logo"><img src="../assets/img/dc-logo.png" alt="header-logo"></div>
<ul>

</ul>
</header>
</template>

<style lang="scss" scoped>
header{
    background-color: white;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}
</style>