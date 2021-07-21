<template>
  <div class="events-section">
    <div class="container py-5"
        data-aos="fade"
        data-aos-duration="1000"
        data-aos-offset="200">
      <!-- title -->
      <div class="section-top text-center">
        <div class="title fw-bold font-times mb-2">Upcoming Events</div>
        <div class="subtitle text-uppercase mb-4">Meet the author in person</div>
      </div>
      <!-- events section -->
      <div class="events mb-5">
        <!-- first event -->
        <div class="event float-start text-center">
          <div class="img-shadow position-relative">
            <img class="w-100" src="../assets/event-05.jpg" alt="#">
            <div class="green-shadow position-absolute w-100 h-100"></div>
          </div>
          <div class="event-name fs-4 pt-4 pb-1">Chicago Book Signing</div>
          <hr class="mx-4">
          <p class="m-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt laborum facere voluptates vel, dolores autem.</p>
        </div>
        <!-- second event -->
        <div class="event float-start text-center">
          <div class="img-shadow position-relative">
            <img class="w-100" src="../assets/event-04.jpg" alt="#">
            <div class="green-shadow position-absolute w-100 h-100"></div>
          </div>
          <div class="event-name fs-4 pt-4 pb-1">Meet &amp; Greet With Amanda</div>
          <hr class="mx-4">
          <p class="m-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt laborum facere voluptates vel, dolores autem.</p>
        </div>
        <!-- third event -->
        <div class="event float-start text-center">
          <div class="img-shadow position-relative">
            <img class="w-100" src="../assets/event-07.jpg" alt="#">
            <div class="green-shadow position-absolute w-100 h-100"></div>
          </div>
          <div class="event-name fs-4 pt-4 pb-1">Open Book: Dialogues</div>
          <hr class="mx-4">
          <p class="m-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt laborum facere voluptates vel, dolores autem.</p>
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
      }

      .subtitle{
        color: $title-yellow;
        font-weight: 600;
        letter-spacing: 1px;
      }
    }

    .events{
      display: table;
      content: '';
      clear: both;

      .event{
        width: calc((100% / 3) - 40px);
        margin: 0 20px;
        background-color: white;

        .img-shadow{
          cursor: pointer;
          transition: 0.3s;

          img{
            transition: 0.3s;
          }

          &:hover .green-shadow{
            background-image: linear-gradient(rgba(239, 247, 233, 0.2), rgba(37, 107, 80, 0.3));
            transition: 0.3s;
          }

          .green-shadow{
            top: 0;
            left: 0;
            transition: 0.3s;
          }
        }

        .event-name{
          transition: 0.5s;
          cursor: pointer;

          &:hover{
            color: $title-yellow;
            text-shadow: 0 10px 30px rgba(90, 90, 90, 0.5);
          }
        }

        hr{
          opacity: 0.15;
        }

        p{
          color: rgba(0, 0, 0, 0.75);
          margin-bottom: 50px;
        }
      }
    }
  }
}

</style>