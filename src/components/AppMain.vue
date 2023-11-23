<script>
export default {
  data(){
    return{
        navItems: [
        {
          title: "DIGITAL COMICS",
          img : "/src/assets/img/digital-comics.png",
          isActive: false,
        },
        {
          title: "DC MERCHANDISE",
          img : "",
          isActive: false,
        },
        {
          title: "SUBSCRIPTION",
          img : "",
          isActive: false,
        },
        {
          title: "COMIC SHOP LOCATOR",
          img : "",
          isActive: false,
        },
        {
          title: "DC POWER VISA",
          img : "",
          isActive: false,
        },
        ],
    };
  },
};


</script>


<template>
<div class="digital">
<ul>
        <li v-for="item in navItems" :key="item">
          <a :class="{ active: item.isActive }" href="">{{ item.title }}</a>
        </li>
  </ul>
</div>
</template>




<style lang="scss" scoped>
.digital{
  background-color: #0282F9;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;

  & ul{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    margin: 0 auto;
    & li{
      list-style: none;
      & a{
        color: white;
        text-decoration: none;
        font-size: 12px;
        font-weight: bold;
        text-transform: uppercase;
        &.active{
          color: #FF0000;
        }
      }
    }
  }
}


</style>