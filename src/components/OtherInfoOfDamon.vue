<template>
  <div class="works-section container p-5">

    <!-- title -->
    <div data-aos="fade-down"
         data-aos-duration="1000"
         data-aos-offset="200">
      <div class="title font-times text-center fw-bold mt-2">Dig A Little Deeper Into Damon Vaughn</div>
      <div class="subtitle text-center text-uppercase pb-5">Find more about the author himself</div>
    </div>

    <!-- info section -->
    <div class="info mb-4 px-5">

      <!-- first info-box -->
      <div class="no-scale-box position-relative d-inline-block"
           data-aos="fade-up-right"
           data-aos-duration="1500"
           data-aos-offset="300">
        <div class="about w-100 h-100">
          <div class="info-shadow w-100 h-100"></div>
        </div>
        <div class="info-text text-white w-75 text-center">
          <div class="fs-3">About Me</div>
          <hr class="position-relative">
          <div>Vestibulum ante ipsum primis</div>
        </div>
      </div>

      <!-- second info-box -->
      <div class="no-scale-box position-relative d-inline-block z-index-3"
           data-aos="fade-up"
           data-aos-duration="1500"
           data-aos-offset="300">
        <div class="latest-book w-100 h-100">
          <div class="info-shadow w-100 h-100"></div>
        </div>
        <div class="info-text text-white w-75 text-center">
          <div class="fs-3">My Latest Book</div>
          <hr class="position-relative">
          <div>Vestibulum ante ipsum primis</div>
        </div>
      </div>

      <!-- third info-box -->
      <div class="no-scale-box position-relative d-inline-block"
           data-aos="fade-up-left"
           data-aos-duration="1500"
           data-aos-offset="300">
        <div class="book-signing w-100 h-100">
          <div class="info-shadow w-100 h-100"></div>
        </div>
        <div class="info-text text-white w-75 text-center">
          <div class="fs-3">Book Signing</div>
          <hr class="position-relative">
          <div>Vestibulum ante ipsum primis</div>
        </div>
      </div>

    </div>

  </div>
</template>

<script>
export default {
    name: 'OtherInfoOfDamon',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.container{
  .title{
    font-size: 40px;
  }
  
  .subtitle{
    letter-spacing: 1px;
    font-size: 18px;
    color: $title-tiffany;
    font-weight: 600;
  }

  .info{

    .no-scale-box{
      width: calc((100% / 3) - 40px);
      height: 400px;
      margin: 0 20px;

      &:hover .about{
        transform: scale(1.03);
      }
      &:hover .latest-book{
        transform: scale(1.03);
      }
      &:hover .book-signing{
        transform: scale(1.03);
      }
    }
    
    .about, .latest-book, .book-signing{
      background-size: cover;
      background-position: left;
      border-radius: 0 0 40px 0;
      transition: 0.3s;
      cursor: pointer;

      &:hover{
        box-shadow: 5px 10px 25px rgb(146, 146, 146);
      }
    }

    .about{
      background-image: url('../assets/box-1.jpg');
    }
    .latest-book{
      background-image: url('../assets/box-4.jpg');
    }
    .book-signing{
      background-image: url('../assets/box-3.jpg');
    }
      
    .info-shadow{
      background-image: linear-gradient(transparent, rgba(0, 0, 0, 0.6));
      border-radius: 0 0 40px 0;
    }

    .info-text{
      cursor: pointer;
      position: absolute;
      bottom: 40px;
      left: 50%;
      transform: translate(-50%);

      hr{
        width: 50px;
        height: 1.5px;
        left: 50%;
        transform: translate(-50%)
      }

      div:last-child{
        color: $title-yellow;
        font-size: 18px;
      }
    }
  }
}

</style>