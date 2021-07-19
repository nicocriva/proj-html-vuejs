<template>
  <div class="sites d-flex align-items-center justify-content-center">
      <a href="#"><img src="../assets/ebay-logotan-2x.png" alt="Ebay logo"></a>
      <a href="#"><img src="../assets/audible-logotan-2x.png" alt="Audible logo"></a>
      <a href="#"><img src="../assets/bb-logotan-2x.png" alt="Barnes and Nobles logo"></a>
      <a href="#"><img src="../assets/kindlefire-logotan-2x.png" alt="Kindle logo"></a>
  </div>
</template>

<script>
export default {
    name: 'SectionOtherSites',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.sites{
  height: 150px;
  background-color: $light-background;
  padding-bottom: 10px;

  a{
    margin: 0 20px;

    img{
      width: 200px;
    }
  } 
  
}

</style>