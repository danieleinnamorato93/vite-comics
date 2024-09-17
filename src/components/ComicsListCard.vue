<script>

export default {
  data() {
    return {
      
    }
  },
  props:{
    comicName:{
        type: String,
        required:true,
    },
    comicImg:{
        type: String,
        required:true,
    }
  }
}
</script>

<template>
<h3>{{ comicName }}</h3>
<img :src=" comicImg " :alt="comicName">

</template>

<style lang="scss" scoped>
img{
    max-width: 150px;
}
</style>