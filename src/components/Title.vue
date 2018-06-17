<template>
   <div class="Title">
      <span class="logo">HaveFun</span>
      <div class="search">
         <i class="fas fa-search"></i>
         <input type="text" placeholder="Explore your own activities">
      </div>
   </div>
</template>

<script>
export default {

}
</script>

<style  lang="scss">
$c-purple: #7828B4;
$c-lightPurple: #9013FE;

.Title{
   width: 100%;
   display: inline-flex;
   align-items: center;
   height: 92px;
   background-color: $c-purple;
   .logo{
      color: white;
      width: 157px;
      height: 44px;
      font-size: 36px;
   }
   .search{
      margin-left: 30px;
      input{
         background: transparent;
         color: white;
         border: none;
         border-bottom: 1px solid white;
         outline: none;
         padding-left: 30px;
         padding-bottom: 5px;
         font-size: 24px;
         width: 360px;
      }
      i{
         &.fa-search{
            font-size: 20px;
            color:white;
            margin-right: -20px;
         }
      }
   }
}
</style>
