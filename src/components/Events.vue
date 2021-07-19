<template>
  <div class="events-section">
    <div class="container py-5">
      <div class="section-top text-center">
        <div class="title font-times mb-2">Upcoming Events</div>
        <div class="subtitle text-uppercase mb-4">Meet the author in person</div>
      </div>
      <div class="events">
        <div class="event text-center">
          <div class="img-shadow position-relative">
            <img class="w-100" src="../assets/event-05.jpg" alt="#">
            <div class="green-shadow position-absolute w-100 h-100"></div>
          </div>
          <div class="fs-5 py-4">Chicago Book Signing</div>
          <hr>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt laborum facere voluptates vel, dolores autem.</p>
        </div>
        <div class="event text-center">
          <div class="img-shadow position-relative">
            <img class="w-100" src="../assets/event-04.jpg" alt="#">
            <div class="green-shadow position-absolute w-100 h-100"></div>
          </div>
          <div class="fs-5 py-4">Chicago Book Signing</div>
          <hr>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt laborum facere voluptates vel, dolores autem.</p>
        </div>
        <div class="event text-center">
          <div class="img-shadow position-relative">
            <img class="w-100" src="../assets/event-07.jpg" alt="#">
            <div class="green-shadow position-absolute w-100 h-100"></div>
          </div>
          <div class="fs-5 py-4">Chicago Book Signing</div>
          <hr>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt laborum facere voluptates vel, dolores autem.</p>
        </div>
        
      </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Events',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.events-section{
  background-color: $light-background;

  .container{
    .section-top {
      .title{
        font-size: 35px;
        font-weight: bold;
      }

      .subtitle{
        color: $title-yellow;
        font-weight: 600;
        letter-spacing: 1px;
      }
    }

    .events{
      width: 100%;
      display: table;
      content: '';
      clear: both;

      .event{
        width: calc((100% / 3) - 40px);
        margin: 0 20px;
        float: left;
        background-color: white;

        .img-shadow{
          cursor: pointer;

          &:hover .green-shadow{
            display: block; 
          }

          .green-shadow{
            background-image: linear-gradient(rgba(239, 247, 233, 0.5), rgba(37, 107, 80, 0.6));;
            top: 0;
            left: 0;
            display: none;
          }
        }
        

        hr{
          opacity: 0.1;
          margin: 0 20px;
        }

        p{
          color: rgba(0, 0, 0, 0.75);
          margin: 20px;
          margin-bottom: 50px;
        }
      }
    }
  }
}

</style>