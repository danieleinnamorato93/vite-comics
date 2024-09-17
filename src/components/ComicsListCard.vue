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
    <div class="container">
        <h3>{{ comicName }}</h3>
        <div class="imgsContainer"><img :src=" comicImg " 
        :alt="comicName"></div>
    </div>


</template>

<style lang="scss" scoped>

h3{
    color: white;
}
.container {
    text-align: center;

    .imgsContainer{
        display: flex;
        justify-content: center;
        img{
    max-width: 100px;
}
    }
}
</style>
