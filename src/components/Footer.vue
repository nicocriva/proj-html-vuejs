<template>
  <footer>
    <div class="container">
      <div class="float-start me-5">
        <img src="../assets/author-logo-round.png" alt="Avada logo">
      </div>
      <div class="float-start w-25 pe-5 me-5">
        <div class="title font-times text-white fw-bold text-uppercase mb-3">About Me</div>
        <div class="about-me-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut fugiat, dignissimos quo delectus, accusantium soluta repudiandae natus, consectetur praesentium quasi tempore rerum reprehenderit. Rerum, ducimus.</div>
      </div>
      <div class="float-start w-25 pe-5 me-5">
        <div class="title font-times text-white fw-bold text-uppercase mb-3">Useful Links</div>
        <div v-for="(item, index) in links" :key="index" class="link-list"><a :href="item.link" class="text-decoration-none"><i class="fas fa-chevron-right me-2"></i> {{item.name}}</a></div>
      </div>
      <div class="float-start w-25 pe-5 me-5">
        
      </div>
      <div> <!-- footer --> </div>
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
          },
          {
            name: 'Subscribe',
            link : 'https://www.google.com/'
          },
          {
            name: 'Social Media',
            link : 'https://www.google.com/'
          }          
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
      width: 150px;
    }

    .about-me-text, .link-list{
      font-size: 12px;
      color: rgba(255, 255, 255, 0.7);
      line-height: 1.8;

      a{
        color: rgba(255, 255, 255, 0.7);
      }
    }
  }
}

</style>