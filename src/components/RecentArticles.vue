<template>
  <div class="section-articles">
    <div class="container">
      
      <!-- header -->
      <header class="d-flex align-items-center justify-content-between">
        <!-- title -->
        <div>
          <h2 class="title font-times">Recent Articles</h2>
          <div class="subtitle text-uppercase">Read the latest entries</div>
        </div>
        <!-- button -->
        <div>
          <button class="border-0 rounded text-white">All Articles</button>
        </div>
      </header>

      <!-- articles section -->
      <div class="articles my-4">
        <!-- first article -->
        <article class="art1 float-start p-4">
          <img class="w-100" src="../assets/20-Tips-scaled.jpg" alt="20 Tips book">
          <div class="article-text p-3">
            <div class="article-title mt-2 fs-5">20 Creativity Tips</div>
              <div class="author">
                By <span>admin</span> | October 24th, 2019 | Categories: <span>Event, Tips &amp; Tricks</span>
              </div>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio in dignissimos sequi natus sunt? Possimus in consequatur pariatur nobis obcaecati?</p>
          </div>
        </article>
        
        <!-- aside column -->
        <aside class="float-start">
          <!-- second article -->
          <article class="art2 p-4">
            <img class="w-100" src="../assets/thumb-13-2x-700x441.jpg" alt="20 Tips book">
            <div class="article-text mt-2">
              <div class="article-title fs-5">What's On Your Booklist?</div>
              <div class="author">
                October 24th, 2019 | <span>3 Comments</span>
              </div>
            </div>
          </article>
          
          <!-- third article -->
          <article class="art3 p-4">
            <img class="w-100" src="../assets/thumb-08-2x-700x441.jpg" alt="20 Tips book">
            <div class="article-text mt-2">
              <div class="article-title fs-5">Istanbul Travel Guide</div>
              <div class="author">
                October 24th, 2019 | <span>2 Comments</span>
              </div>
            </div>
          </article>
        </aside>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'RecentArticles',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.section-articles{
  background-color: #fef7e9;
  padding: 80px 210px;
  
  .container{
    header{
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

      .art1, aside{
        height: 620px;
        background-color: white;
      }

      .art1{
        width: calc(70% - 20px);
        margin-right: 20px;
      }

      aside{
        width: calc(30% - 20px);
        margin-left: 20px;
      }

      img{
        transition: 0.5s;
                
        &:hover{
          z-index: -1;
          overflow: hidden;
          transform: scale(1.05)
        };
      }

      .article-title{
        transition: 0.2s;
        cursor: pointer;
        
        &:hover{
          color: $title-yellow;
        }
      }

      .author{
        font-size: 12px;
        color: rgb(90, 90, 90);
        margin: 10px 0 20px;

        span {
          color: black;
          transition: 0.2s;
          cursor: pointer;

          &:hover{
            color: $title-yellow;
          }
        }
      }

      p{
        color: rgb(90, 90, 90);
      }
    }
  }  
}

</style>