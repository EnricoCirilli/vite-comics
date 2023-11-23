<script>
export default {
  data() {
    return {
      navItems: [
        {
          title: "CHARACTERS",
          isActive: false,
        },
        {
          title: "COMICS",
          isActive: true,
        },
        {
          title: "MOVIES",
          isActive: false,
        },
        {
          title: "TV",
          isActive: false,
        },
        {
          title: "GAMES",
          isActive: false,
        },
        {
          title: "COLLECTIBLES",
          isActive: false,
        },
        {
          title: "VIDEOS",
          isActive: false,
        },
        {
          title: "FANS",
          isActive: false,
        },
        {
          title: "NEWS",
          isActive: false,
        },
        {
          title: "SHOP",
          isActive: false,
        },
        
      ],
   
    }
  },
}

</script>


<template>

<header>
  <div class="logo">
  <img src="src/assets/img/dc-logo.png" alt="">
  </div>
<nav>
  <ul>
        <li v-for="item in navItems" :key="item.title">
          <a :class="{ active: item.isActive }" href="">{{ item.title }}</a>
        </li>
  </ul>
</nav>
</header>
</template>


<style lang="scss" scoped>
header {
  width: 80%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}
ul{
  display: flex;
  justify-content: space-between;
  align-items: center;
  list-style: none;
  padding: 0;
  margin: 0;
}
li{
  margin: 0 10px;
}
a{
  text-decoration: none;
  color:black;
  font-size: 14px;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 1px;
  padding: 10px;
  border-radius: 5px;
}



</style>