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
    <div class="comic-item">
       
        <img :src=" comicImg " 
        :alt="comicName">
        <h3>{{ comicName }}</h3>
    </div>


</template>

<style lang="scss" scoped>

h3{
    color: white;
    font-size: 13px;
   
    
   
}
.comic-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    height: 250px;
    width: calc(100% / 6);
   
    box-sizing: border-box;

    img {
        max-width: 130px;
        max-height: 190px;
        object-fit: contain;
        padding-bottom: 20px;
        padding-top: 7px;
    }
    
}

    
</style>
