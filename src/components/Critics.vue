<template>
  <div class="critics-section w-75 container px-4 overflow-hidden">

    <div class="critics-header d-flex align-items-center justify-content-between"
        data-aos="fade-down"
        data-aos-duration="1000"
        data-aos-offset="200">
      <div>
        <!-- title -->
        <h2 class="title font-times">What The Critics Say</h2>
        <div class="subtitle  text-uppercase">Testimonial From Around The World</div>
      </div>
      <!-- button -->
      <div>
        <button class="border-0 rounded text-white">Read All Testimonial</button>
      </div>
    </div>

    <!-- articles section -->
    <div class="articles mt-4"
        data-aos="fade-left"
        data-aos-duration="1000"
        data-aos-offset="200">

      <!-- first article -->
      <div class="no-scale-box float-start position-relative">
        <div class="art1">
          <div class="img-shadow w-100 h-100">
            <!-- article text -->
          </div>
        </div>

        <div class="art-text position-absolute text-white w-100">

          <h2 class="title font-times text-bold"> Best Author Of His Generation </h2>
          <hr>
          <h5 class="subtitle my-4">This book will change yoru perspective on life</h5>
          <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi culpa sequi architecto eaque eligendi quibusdam laborum labore ut unde eum magni iste error perspiciatis praesentium harum, ex soluta veniam dicta?</p>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus quaerat sint temporibus reprehenderit est sequi eum reiciendis eius ad excepturi? Facere ad id quod? Necessitatibus!</p>
          <div class="mt-5">
            <img class="d-inline-block me-3" src="../assets/nytimes-logo-white-xsmall.png" alt="New York Times logo">
            <div class="d-inline-block light-bold">Justine Kilpatrick, <span class="article-author">The New York Times</span></div>
          </div>

        </div>
      </div>

      <!-- second article -->
      <article class="art2 float-end">
        <div class="article-content p-4 text-center mb-2">
          <!-- article text -->
          <h5 class="title font-times fs-4">A True Masterpiece, Bravo!</h5>
          <p class="mx-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, provident quam tempore animi iusto voluptas modi dignissimos impedit deleniti aut! Minima tenetur quo commodi et ipsam magnam, facilis corrupti! Dolorum porro quaerat!</p>
        </div>
        <div class="mb-5 pt-2">
          <img src="../assets/theguardian-xsmall.png" alt="The Guardian logo">
          <div class="ms-4 d-inline-block text-secondary fw-bold  ">Gerald Hendley, <span class="text-dark fw-normal">The Guardian</span></div>
        </div>
      </article>

      <!-- third article -->
      <article class="art3 mt-2 float-end">
        <div class="article-content p-4 text-center mb-2">
          <!-- article text -->
          <h5 class="title font-times fs-4">A Unique View On The World</h5>
          <p class="mx-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, provident quam tempore animi iusto voluptas modi dignissimos impedit deleniti aut! Minima tenetur quo commodi et ipsam magnam, quos natus doloribus neque nostrum, illum, quo temporibus tempore porro quaerat!</p>
        </div>
        <div class="mb-5 pt-2">
          <img src="../assets/globe-xsmall.png" alt="The Guardian logo">
          <div class="ms-4 d-inline-block text-secondary fw-bold  ">Mary Maxey, <span class="text-dark fw-normal">The Globe And Mail</span></div>
        </div>
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
  padding: 50px 0 50px 0;

  .critics-header{
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
    display: table;
    content: '';
    clear: both;
    height: 600px;

    .no-scale-box{
      height: 700px;
      width: 60%;
      cursor: pointer;

      &:hover .art1{
        transform: scale(1.03);
      }

      .art1{
        width: 100%;
        height: 100%;
        background-image: url('../assets/testimonial2-2x.jpg');
        background-size: cover;
        border-radius: 0 0 80px 0;
        transition: 0.3s;
      }

      .img-shadow{
        background-color: rgba(0, 0, 0, 0.2);
        border-radius: 0 0 80px 0;
        padding: 90px;
      }
          
      .art-text{
        padding: 70px 100px;
        top: 50%;
        transform: translate(-0%, -50%);

        .title{
          font-weight: 600;
          font-size: 40px;
        }

        hr{
          opacity: 0.5;
          margin: 30px 0;
        }
  
        .light-bold{
          font-weight: 600;
         
          .article-author{
            color: $title-tiffany;
          }
        }
      }
    }

    .art2, .art3{
      width: 35%;
    }

    .article-content{
      background-color: $light-background;  
      
      .title{
        font-weight: 600;
      }

      p{
        line-height: 1.6;
        color: rgba(0, 0, 0, 0.65);
      }
    }
  }
}

</style>