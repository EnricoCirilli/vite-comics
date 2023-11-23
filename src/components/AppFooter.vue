<script>
export default {
  data(){
    return{
      navItems: [
        {
          subtitle: "Characters" },
        {
          subtitle: "Comics"
        },
        {
          subtitle: "Movies"
        },
        {
          subtitle: "TV"
        },
        {
          subtitle: "Games"
        },
        {
          subtitle: "Videos"
        },
        {
          subtitle: "News"
        },
        {
          subtitle: "Shop"
        },
      ],

      navShop: [
        {
          subtitle: "Shop DC" },
        {
          subtitle: "Shop DC Collectibles",
        },
      
      ],

      navDc: [
        {
          subtitle: "Terms of Use" },
        { subtitle: "Privacy Policy (New updated)" },
        { subtitle: "Ad Choices" },
        { subtitle: "Advertising" },
        { subtitle: "Jobs" },
        { subtitle: "Subscriptions" },
        { subtitle: "Talent Workshops" },
        { subtitle: "CPSC Certificates" },
        { subtitle: "Ratings" },
        { subtitle: "Shop Help" },
        { subtitle: "Contact Us" },
        
      
      ],
      navSites: [
        {
          subtitle: "DC" },
        { subtitle: "MAD Magazine" },
        { subtitle: "DC Kids" },
        { subtitle: "DC Universe" },
        { subtitle: "DC Power Visa" },
       
      ],

    };
  },
};


</script>


<template>
<div class="footer">
  <div class="row">
    <div class="col">
  <ul>
        <h4>DC COMICS</h4>
        <li v-for="item in navItems" :key="item.subtitle">
          <a :class="{ active: item.isActive }" href="">{{ item.subtitle }}</a>
        </li>
  </ul>
  <ul>
        <h4>SHOP</h4>
        <li v-for="item in navShop" :key="item.subtitle">
          <a :class="{ active: item.isActive }" href="">{{ item.subtitle }}</a>
        </li>
  </ul>
    </div>
    <div class="col">
  <ul>
        <h4>DC</h4>
        <li v-for="item in navDc" :key="item.subtitle">
          <a :class="{ active: item.isActive }" href="">{{ item.subtitle }}</a>
        </li>
  </ul>
    </div>
    <div class="col">
  <ul>
        <h4>SITES</h4>
        <li v-for="item in navSites" :key="item.subtitle">
          <a :class="{ active: item.isActive }" href="">{{ item.subtitle }}</a>
        </li>
  </ul>
    </div>
<img src="src/assets/img/dc-logo-bg.png" alt="">

</div>
</div>
</template>




<style lang="scss" scoped>
.footer{
background-image: url(src/assets/img/footer-bg.jpg) ;
background-size: cover;
background-repeat: no-repeat;
height: 450px;
 & img{
  display: block;
     margin-left: 10%;
      max-height:350px;
 };
 .row{
   display: flex;
   flex-direction: row;
    justify-content: space-between;
    padding: 60px;
    & .col{
      display: flex;
      flex-direction: column;
    
      & ul{
        list-style: none;
        & li{
          list-style: none;
          & a{
            color: lightgrey;
            text-decoration: none;
            font-size: 10px;
            font-weight: bold;
          };
        };
      };
    };
  }
 h4{
       color: white;
       font-size: 20px;
       font-weight: bold;
     };
};



</style>