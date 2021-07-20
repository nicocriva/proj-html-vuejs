<template>
  <div class="works-section container p-5">
    <div class="title font-times text-center fw-bold mt-2">Dig A Little Deeper Into Damon Vaughn</div>
    <div class="subtitle text-center text-uppercase pb-5">Find more about the author himself</div>
    <div class="info mb-4 px-5">
      <div class="about d-inline-block position-relative">
        <div class="info-shadow w-100 h-100">
          <div class="info-text w-100 text-center position-absolute">
            <div class="text-white fs-3">About Me</div>
            <hr class="position-relative text-white">
            <div>Vestibulum ante ipsum primis</div>
          </div>
        </div>
      </div>
      <div class="latest-book d-inline-block position-relative">
        <div class="info-shadow w-100 h-100">
          <div class="info-text w-100 text-center position-absolute">
            <div class="text-white fs-3">My Latest Book</div>
            <hr class="position-relative text-white">
            <div>Vestibulum ante ipsum primis</div>
          </div>
        </div>
      </div>
      <div class="book-signing d-inline-block position-relative">
        <div class="info-shadow w-100 h-100">
          <div class="info-text w-100 text-center position-absolute">
            <div class="text-white fs-3">Book Signing</div>
            <hr class="position-relative text-white">
            <div>Vestibulum ante ipsum primis</div>
          </div>
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

    .about, .latest-book, .book-signing{
      width: calc((100% / 3) - 40px);
      height: 400px;
      margin: 0 20px;
      background-size: cover;
      background-position: center;
      border-radius: 0 0 40px 0;
      transition: 0.3s;
      cursor: pointer;

      &:hover{
        transform: scale(1.03);
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

        .info-text{
          bottom: 40px;
          left: 50%;
          transform: translate(-50%);

          hr{
            width: 50px;
            height: 2px;
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
}

</style>