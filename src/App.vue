<template>
  <div id="app">
    <Header/>
    <main>
      <MoreAboutDamon/>
      <SectionOtherSites/>
      <JumbotronAudiobook/>
      <Critics/>
      <Events/>
      <JumbotronSubscribe/>
      <OtherInfoOfDamon/>
      <RecentArticles/>
    </main>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MoreAboutDamon from './components/MoreAboutDamon.vue'
import SectionOtherSites from './components/SectionOtherSites.vue'
import JumbotronAudiobook from './components/JumbotronAudiobook.vue'
import Critics from './components/Critics.vue'
import Events from './components/Events.vue'
import JumbotronSubscribe from './components/JumbotronSubscribe.vue'
import OtherInfoOfDamon from './components/OtherInfoOfDamon.vue'
import RecentArticles from './components/RecentArticles.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    MoreAboutDamon,
    SectionOtherSites,
    JumbotronAudiobook,
    Critics,
    Events,
    JumbotronSubscribe,
    OtherInfoOfDamon,
    RecentArticles,
    Footer
  }
}
</script>

<style lang="scss">
@import 'bootstrap';
@import './style/commons.scss';
@import 'style/vars.scss';
@import url('https://fonts.googleapis.com/css2?family=Kristi&display=swap');

</style>
