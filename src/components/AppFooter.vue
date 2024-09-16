<script>
export default {
  data() {
    return { 
      socialLogos: [{
        
        logo:'footer-facebook.png'
      },
      {
     
        logo:'footer-periscope.png'
      },

      {
        
        logo:'footer-pinterst.png'
      },

      {
       
        logo:'footer-twitter.png'
      },
      {
        
        logo:'footer-youtube.png'
      },


      ]

      
    };
  },
  methods: {
    getImagePath: function(imgPath) {
      return new URL(`../assets/img/${imgPath}`, import.meta.url).href;
    }
}
}
</script>

<template>
  <footer>
    <div class="button"><a href="#"><button>SIGN-UP NOW!</button></a></div>
    <div class="social">
     
      <ul>
        <span><h4>FOLLOW US!</h4></span>
        <li v-for="mark in socialLogos"><a href="#">
          <img :src="getImagePath(mark.logo)" alt=""></a>
         
          </li>
      </ul>

    </div>
  </footer>

</template>

<style lang="scss" scoped>
footer {
  height: 150px;
  background-color: #303030;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
}
ul {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 20px;
  gap: 7px;
  img {
    height: 25px;}
    h4{
      color: #0282F9;;
    }
}
button {
  border: 1px solid blue;
  background-color: transparent;
  color: white;
  text-align: center;
  padding: 10px;

}

</style>