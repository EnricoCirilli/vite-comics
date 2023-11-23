<script>
export default {
  data(){
    return{};
  },
};


</script>


<template>
<div class="cta">
<button> SIGN UP NOW!</button>

  <ul>
    <li>
      <a href="">FOLLOW US</a>
     <a href=""><img src="src/assets/img/footer-facebook.png" alt=""></a>
     <a href=""><img src="src/assets/img/footer-twitter.png" alt=""></a>
     <a href=""><img src="src/assets/img/footer-youtube.png" alt=""></a>
     <a href=""><img src="src/assets/img/footer-periscope.png" alt=""></a>
    </li>
  </ul>

</div>
</template>




<style lang="scss" scoped>
.cta{
  display: flex;
  justify-content: space-between;
  background-color: rgb(56, 53, 53);
  padding: 60px;
  border: 1px solid #0282F9;

  & button{
    background-color: rgb(56, 53, 53);
    border: 1px solid #0282F9;
    color: white;
   
    padding: 10px 20px;
    border-radius: 5px;
    display: block;
  }
  & ul{
    display: flex;
    justify-content: space-between;
    align-items: center;
    list-style: none;
    & li{
      display: flex;
      justify-content: space-between;
      align-items: center;
      & a{
        color: white;
        text-decoration: none;
        font-size: 12px;
        font-weight: bold;
        margin-right: 10px;
      }
    }
  }


}


</style>