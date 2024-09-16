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
  min-height: 100px;
}
ul{
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  text-align: center;
}
li {
  text-align: center;
}
img{
  filter: invert(0%);
  height: 30px;

}
</style>