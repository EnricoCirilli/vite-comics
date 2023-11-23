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
<p>x</p>
<ul>
        <li v-for="item in navItems" :key="item">
          <a :class="{ active: item.isActive }" href="">{{ item.title }}</a>
        </li>
  </ul>
</div>
</template>




<style lang="SCSS" scoped>
.digital{
  border: 1px red solid;
  background-color: rgb(136, 136, 220);
}


</style>