<template>
  <header class="vh-100">
    <div class="opacity-shadow">
      <div class="header-top d-flex justify-content-between align-items-center">
        <div class="avada-logo h-100">
          <img class="h-100" src="../assets/author-logo-round.png" alt="">
        </div>
        <div class="header-nav">
          <ul class="list-unstyled">
            <li class="d-inline-block mx-3 mb-4" v-for="(item, index) in navBar" :key="index">
              <a href="#" class="list-unstyled text-decoration-none">{{item}}</a>
            </li>
            <li class="d-inline-block mx-3 mb-4">
              <a href="#" class="list-unstyled text-decoration-none"><i class="fas fa-shopping-cart"></i></a>
            </li>
          </ul>
        </div>
      </div>
      <div class="header-bottom">
        <div>
          <!-- left content -->
        </div>
        <div>
          <!-- latest book -->
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      navBar: ['Home', 'About', 'Testimonials', 'My Blog', 'Meetups', 'Shop', 'Contact Me']
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{
  background-image: url(../assets/hero-07-2x.jpg);
  background-size: cover;
  background-position: center;
  background-repeat:no-repeat;

  .opacity-shadow{
    height: 100%;
    background-color: rgba(0, 0, 0, 0.2);
    background-image: linear-gradient(transparent, rgba(0, 0, 0, 0.7));

    .header-top{
      width: 90%;
      height: 120px;
      margin: 0 auto;

      a{
        color: white;
        padding: 25px 0;
        transition: 0.5s;
        font-weight: 400;           
        border-top: 5px solid transparent;
  
        &:hover {
          color: #edaf29;     
          border-top: 5px solid #edaf29;
        }
      }
    }
  }
}
</style>
