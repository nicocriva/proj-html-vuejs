<template>
  <div class="jumbo-sub text-center">
    <!-- dark jumbo shadow  -->
    <div class="jumbo-shadow">
      <div class="container py-5">
        <!-- title -->
        <div class="title font-times pt-1 mt-4 text-white">
          Subscribe To My Newsletter
        </div>
        <div class="subtitle text-uppercase">
          be notified about book signing tour dates
        </div>
        <!-- form -->
        <form action="">
          <input class="p-2 rounded border-0 mx-2" type="email" placeholder="Inserisci la tua mail">
          <button class="p-2 px-5 rounded border-0 text-white">Subscribe</button>
        </form>
        <div class="mt-4 mb-5">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aliquam, dignissimos.</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'JumbotronSubscribe',
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.jumbo-sub{
  background-image: url('../assets/banner-2.jpg');
  background-size: cover;

  .jumbo-shadow{
    background-color: rgba(0, 0, 0, 0.2);
  }

  .container{
    width: 35%;

    .title{
      font-size: 35px;
      font-weight: 500;
    }

    .subtitle{
      font-size: 14px;
      font-weight: 600;
      color: $title-yellow;
      letter-spacing: 1px;
      margin: 10px 0 25px 0;
    }

    form{
      button{
        background-color: $title-tiffany;

        &:hover{
          background-color: #297268;
        }
      }
    }

    div:last-child{
      color: rgba(160, 160, 160, 0.8);
      font-size: 13px;
    }
  }
  
}

</style>