<template>
  
  <div class="damon-info d-flex flex-column align-items-center justify-content-center my-4"
      data-aos="fade-down"
      data-aos-duration="1500"
      data-aos-offset="200">
    
    <!-- title -->
    <div class="title font-kristi">
      More About Damon Vaughn
    </div>
    <div class="info">
      Damon Vaughn is a professor of psychology at the University of Toronto, a clinical psychologist and the author of the multi-milon copy bestseller "The story of my life."
    </div>

    <!-- button -->
    <div>
      <button class="border-0 my-4 text-white rounded">Meet The Author</button>
    </div>
  </div>

</template>

<script>
export default {
    name: 'MoreAboutDamon',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.damon-info{
  height: 350px;
  width: 70%;
  margin: 0 auto;

  .title{
    font-size: 75px;
    color: $title-yellow;
  }

  .info{
    text-align: center;
    font-size: 25px;
  }

  button{
    font-size: 14px;
    font-weight: 600;
    padding: 10px 15px;
    background-color: $title-tiffany;
    transition: 0.2s;


    &:hover{
      background-color: #297268;
    }
  }
}

</style>