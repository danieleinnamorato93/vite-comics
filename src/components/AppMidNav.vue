<script>
export default {
  data() {
    return {
      links: [{
      name:"DIGITAL COMICS",
      avatar:'buy-comics-digital-comics.png'
      },
      {
      name:"DC MERCHANDISE",
      avatar:'buy-comics-merchandise.png'
      },
      {
      name:"SUBSCRIPTION",
      avatar:'buy-comics-subscriptions.png'
      },
      {
      name:"COMIC SHOP LOCATOR",
      avatar:'buy-comics-shop-locator.png'
      },
      {
      name:"DC POWER VISA",
      avatar:'buy-dc-power-visa.svg'
      }
      
        
      ]
    };
  },
  methods: {
    getImagePath: function(imgPath) {
      return new URL(`../assets/img/${imgPath}`, import.meta.url).href;
    }
  }
};
</script>

<template>
  
  <section>
    <ul>
  <li v-for="link in links" :key="link.name">
 <img :src="getImagePath(link.avatar)" alt="link.name">
 <span>{{ link.name }}</span>
</li>
</ul>

  </section>

</template>

<style lang="scss" scoped>
section{
  background-color: #0282F9;
  min-height: 150px;
  display: flex;
  justify-content: space-between;
  align-items: center;

}
ul{
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  text-align: center;
  justify-content: center;
 
}
li {
  display: flex;

  margin: 0 15px;
  
}
img{
  filter: invert(0%);
  height: 35px;
  margin-right: 10px ;

}
span {
  color: white;
  font-size: 12px;
  line-height: 35px;
}
</style>