<template>
  <div class="app-container">
    <TheHeader/>


    <div class="app-content">
      <nuxt/>
    </div>

    <TheFooter/>
  </div>
</template>

<script>
import TheHeader from '~/components/templateMonster/TheHeader'
import TheSideNav from '~/components/templateMonster/TheSideNav'
import TheFooter from '~/components/templateMonster/TheFooter'
export default {
  components: {
    TheHeader,
    TheSideNav,
    TheFooter
  }
}
</script>

<style>
    html, body{
        margin: 0;
        height: 100%;
        width: 100%;
    }
    .app-container{
        position: relative;
        display: grid;
        grid-template: auto 1fr auto / 1fr;
    }
    .app-content{
        min-height: 88.5vh;
        padding: 24px;
        display: grid;
    }
</style>