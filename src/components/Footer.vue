<template>
  <footer class="position-relative">
    <div class="container">
      <div class="float-start me-5">
        <img src="../assets/author-logo-round.png" alt="Avada logo">
      </div>
      <div class="float-start w-25 pe-5 me-3">
        <div class="title font-times text-white fw-bold text-uppercase mb-3">About Me</div>
        <div class="about-me-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut fugiat, dignissimos quo delectus, accusantium soluta repudiandae natus, consectetur praesentium quasi tempore rerum reprehenderit. Rerum, ducimus.</div>
      </div>
      <div class="float-start w-25 pe-5 me-3">
        <div class="title font-times text-white fw-bold text-uppercase mb-3">Useful Links</div>
        <div v-for="(item, index) in links" :key="index" class="link-list mb-2">
          <a :href="item.link" class="text-decoration-none"><i class="fas fa-chevron-right text-white me-2"></i> {{item.name}} </a>
        </div>
      </div>
      <div class="float-start w-25 pe-5 me-3">
        <div class="title font-times text-white fw-bold text-uppercase mb-3">Contact Info</div>
        <div v-for="(item, index) in contacts" :key="index" class="link-list mb-2">
          <div>{{item.name}}</div>
        </div>
        <div v-for="item in social" :key="item.name" class="d-inline-block mx-1 social-icon">
          <a href="#"><i :class="item.name"></i></a>
        </div>
      </div>
    </div>
    <div class="credits w-100 text-center position-absolute">
      &copy; Copyright 2012 - 2021 | Avada Theme by <strong class="text-white">ThemeFusion</strong> | All Rights Reserved | Powered by <strong class="text-white">WordPress</strong>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    data(){
      return{
        links: [
          {
            name: 'Latest Books',
            link : 'https://www.google.com/'
          },
          {
            name: 'Upcoming Events',
            link : 'https://www.google.com/'
          },
          {
            name: 'Recent Articles',
            link : 'https://www.google.com/'
          },
          {
            name: 'Business Enriquiries',
            link : 'https://www.google.com/'
          },
          {
            name: 'Visit My Foundation',
            link : 'https://www.google.com/'
          },
          {
            name: 'Book Signing',
            link : 'https://www.google.com/'
          }  
        ],

        contacts: [
          {
            name: '63 E. Studebaker Street Bolingbrook, IL 60440',
          },
          {
            name: 'Phone: (800) 000-0000',
          },
          {
            name: 'Mobile: (800) 000-0000'
          },
          {
            name: 'Email: info@your-company.com'
          }
        ],

        social: [
          {
            name: 'fab fa-facebook-f',
          },
          {
            name: 'fab fa-twitter',
          },
          {
            name: 'fab fa-instagram',
          },
          {
            name: 'fab fa-linkedin',
          },
          {
            name: 'fab fa-youtube',
          },
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

footer{
  height: 450px;
  padding: 100px 0;
  background-image: url('../assets/footer-3.jpg');
  background-size: cover;
  background-position: top;

  .container{
    display: table;
    clear: both;
    content: '';

    img{
      width: 130px;
    }

    .title{
      letter-spacing: 1px;
    }

    .about-me-text, .link-list{
      font-size: 14px;
      color: rgba(255, 255, 255, 0.7);
      line-height: 1.8;

      a{
        color: rgba(255, 255, 255, 1);
        margin: 50px 0;
        transition: 0.3s;

        &:hover{
          color: $title-yellow;
        }
      }
    }
    .social-icon a{
      color: rgba(255, 255, 255, 0.7);
      font-size: 18px;

      i{
        margin: 20px 5px;
      }

      &:hover{
        color: white;
      }
    }
  }
  .credits{
    color: rgba(255, 255, 255, 0.7);
    bottom: 30px;
    font-size: 12px;
  }
}

</style>