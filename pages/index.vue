<template>
  <div>
    <AppHeader @changeSite='changeSite($event)'/>
    <Home v-if="pageNumber == 0" @changeSite='changeSite($event)'/>
    <Info v-if="pageNumber == 1"/>
    <Contact v-if="pageNumber == 4"/>
  </div>
</template>

<script>
import AppHeader from '~/components/AppHeader'
import Home from '~/components/Home'
import Info from '~/components/Info'
import Contact from '~/components/Contact'

export default {
  data(){
    return{
      pageNumber: 0,
    }
  },
  methods:{
    changeSite(pageNumber1){
      this.pageNumber = pageNumber1; 
    }
  }
}
</script>

<style scoped>
div{
  height: 100%;
}
</style>