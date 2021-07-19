<template>
  <div class="critics-section container">
    <div class="critics-header d-flex align-items-center justify-content-between">
      <div>
        <h2 class="title font-times">What The Critics Say</h2>
        <div class="subtitle text-uppercase">Testimonial From Around The World</div>
      </div>
      <div>
        <button class="border-0 rounded text-white">Read All Testimonial</button>
      </div>
    </div>
    <div class="articles mt-4">
      <article class="art1 text-white">
        <div class="img-shadow">
          <h2 class="title font-times text-bold"> Best Author Of His Generation </h2>
          <hr>
          <h5 class="subtitle">This book will change yoru perspective on life</h5>
          <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi culpa sequi architecto eaque eligendi quibusdam laborum labore ut unde eum magni iste error perspiciatis praesentium harum, ex soluta veniam dicta?</p>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus quaerat sint temporibus reprehenderit est sequi eum reiciendis eius ad excepturi? Facere ad id quod? Necessitatibus!</p>
          <div class="mt-5">
            <img class="d-inline-block me-3" src="../assets/nytimes-logo-white-xsmall.png" alt="New York Times logo">
            <div class="d-inline-block">Justine Kilpatrick, <span class="article-author">The New York Times</span></div>
          </div>
        </div>
      </article>
      <article class="art2 text-center">
        <h5 class="title font-times fs-4">A True Masterpiece, Bravo!</h5>
        <p class="">Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, provident quam tempore animi iusto voluptas modi dignissimos impedit deleniti aut! Minima tenetur quo commodi et ipsam magnam, maxime natus excepturi facere quas quis laudantium facilis corrupti! Dolorum corrupti aperiam voluptatem tenetur modi voluptate quos natus doloribus neque nostrum, illum, quo temporibus tempore porro quaerat!</p>
      </article>
      <article class="art3">
        art3
      </article>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Critics',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.critics-section{
  height: 1000px;
  width: 75%;
  padding: 50px 0 100px 0;

  .critics-header{
    width: 100%;

    .title{
      font-weight: 600;
      font-size: 40px;
    }

    .subtitle{
      color: $title-tiffany;
      font-weight: 600;
      font-size: 18px;
      letter-spacing: 1px;
    }

    button{
      padding: 10px 30px;
      background-color: $title-yellow;
      font-weight: 600;

      &:hover{
      background-color: #eba206;
      }
    }
  }

  .articles{
    height: calc(100% - 100px);
    width: 100%;

    .art2, .art3{
      float: right;
    }

    .art1{
      width: 60%;
      height: 90%;
      float: left;
      background-image: url('../assets/testimonial2-2x.jpg');
      background-size: cover;
      border-radius: 0 0 80px 0;

      .img-shadow{
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.2);
        border-radius: 0 0 80px 0;
        padding: 90px;
      
        .title{
          font-weight: 600;
          font-size: 40px;
        }

        .subtitle{
          margin: 30px 0;
        }

        hr{
          opacity: 0.5;
          margin: 30px 0;
        }

        .article-author{
          color: $title-tiffany;

        }
      }

    }

    .art2, .art3{
      width: 35%;
      padding: 30px;
      // background-color: darkgoldenrod;
    }

    .art2{
      margin-bottom: 30px;
      background-color: $light-background;
      
      .title{
        font-weight: 600;
      }

      p{
        // font-size: 18px;
        line-height: 1.6;
        color: rgba(0, 0, 0, 0.65);
      }
    }
  }
  
}

</style>