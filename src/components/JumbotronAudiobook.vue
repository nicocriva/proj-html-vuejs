<template>
  <div class="jumbo-book">
    <div class="container h-100 d-flex overflow-hidden align-items-center">
      <!-- phone image -->
      <div class="phone-img w-50 h-100"
          data-aos="fade-up"
          data-aos-duration="1500"
          data-aos-offset="400">
        <img class="h-100 pt-5" src="../assets/audible-app-2x.png" alt="Audible app">
      </div>
      <!-- jumbo text -->
      <div class="new-audiobook text-center"
          data-aos="fade-left"
          data-aos-duration="1500"
          data-aos-offset="300">
        <h2 class="title text-light font-times">New Audiobook</h2>
        <div class="subtitle text-uppercase">No time to read? No problem, listen to it</div>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae, excepturi ratione odio?</p>
        <!-- web sites logo -->
        <a href="#"><img src="../assets/audible-logo.png" alt="Audible logo"></a>
        <a href="#"><img src="../assets/bn-logo-tall.png" alt="Bn logo"></a>
        <a href="#"><img src="../assets/kindle-logo-tall.png" alt="Kindle logo"></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'JumbotronAudiobook',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.jumbo-book{
  height: 450px;
  background-image: url('../assets/banner.jpg');
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;

  .container{
    width: 70%;

    .new-audiobook{
      .title{
        font-weight: 600;
        font-size: 40px;
      }

      .subtitle{
        color: $title-yellow;
        font-weight: 600;
      }

      p{
        font-size: 14px;
        margin: 20px 100px;
        color: rgba(255, 255, 255, 0.7)
      }

      img{
        width: 120px;
        margin: 0 20px;
        transition: 0.5s;

        &:hover{
          transform: scale(1.05);
        }
      }
    }
  }
}

</style>