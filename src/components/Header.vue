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
      <div class="header-bottom w-100 position-relative">
        <div class="btm-left position-absolute">
          <h2 class="font-kristi">Damon Vaughn</h2>
          <p class="quote text-light font-times">Best-selling author and the most influential public intellectual in the western world right now.</p>
          <p class="quote-author">- The New York Times</p>
          <div class="slider-buttons mt-4 text-light d-flex justify-content-center align-items-center">
            <div><i class="fas fa-arrow-left"></i></div>
            <div><i class="fas fa-arrow-right"></i></div>
          </div>
        </div>
        <div class="btm-right position-absolute">
          <img src="../assets/book-widget.png" class="float-start" alt="book">
          <div class="float-start w-50 mt-2">
            <div class="latest-book font-times mb-2 fs-4">Latest Book Release</div>
            <div class="latest-book-name color-yellow">D: VAUGHN AUTOBIOGRAPHY</div>
            <div class="latest-book-description">Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae sit incidunt quasi nam.</div>
          </div>
          <div class="buy-buttons rounded w-100">
            <button class="w-50 float-start"> <i class="fab fa-amazon"></i> Buy On Amazon</button>
            <button class="w-50 float-start"> <i class="fab fa-apple"></i> Buy On AppStore</button>
            <!-- <div class="w-50 float-start">amazon</div>
            <div class="w-50 float-start">apple</div> -->
          </div>
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
@import '../style/vars.scss';

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
          color: $title-yellow;     
          border-top: 5px solid $title-yellow;
        }
      }
    }

    .header-bottom{
      height: calc(100vh - 120px);

      .btm-left{
        width: 600px;
        height: 400px;
        bottom: 100px;
        left: 150px;

        h2{
          font-size: 80px;
          color: $title-yellow;
        }

        .quote{
          font-size: 35px;
          font-weight: bold;
        }

        .quote-author{
          font-size: 20px;
          color: rgba(255, 255, 255, 0.5);
          font-style: italic;
        }

        .slider-buttons{
          width: 80px;
          height: 35px;

          & div{
            background-color: rgba(0, 0, 0, 0.4);
            font-size: 12px;
            padding: 10px 15px;
            margin-left: 1px;
            cursor: pointer;
            transition: 0.3s;

          }

          & div:active i{
            transform: scale(1.3);
            transition: 0.1s;
          }

          & div:hover{
            color: black;
            background-color: white;
          }

          & div:first-child{
            border-radius: 5px 0 0 5px;
          }

          & div:last-child{
            border-radius: 0 5px 5px 0;
          }
        }
      }

      .btm-right{
        width: 35%;
        height: 350px;
        padding: 40px 50px;
        bottom: 0;
        right: 0;
        background-color: rgb(255, 255, 255);
        

        & img{
          width: 50%;
        }

        .latest-book{
          font-weight: 600;
        }

        .latest-book-description{
          font-size: 14px;
          color: rgba(0, 0, 0, 0.7);
          margin-top: 15px;
          line-height: 1.6;
          margin-bottom: 50px;
        }

        .buy-buttons {
          width: 100%;
          line-height: 30px;
          display: table;
          clear: both;
          content: '';
          box-shadow: 0 15px 100px #888888;

          & button:first-child{
            border-radius: 5px 0 0 5px;

            &:hover{
              border: 1px solid rgb(92, 214, 92);
              background-color: white;
            }
          }

          & button:last-child{
            border-radius: 0 5px 5px 0;

            &:hover{
              border: 1px solid rgb(92, 214, 92);
            }
          }

          & button {
            padding: 5px;
            font-size: 13px;
            border: 1px solid rgba(112, 170, 112, 0.555);
            transition: 0.3s;
            background-color: #f1fdf9;
          }
          
        }
      }
    }
  }
}
</style>
