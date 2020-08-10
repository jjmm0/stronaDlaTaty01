<template>

<div class="navblock">
  <div class="wrapper2">
    <!-- <div @click="linkNumberChange(0)"><p class="main" >Główna</p></div>
    <div @click="linkNumberChange(1)"><p class="main" >Główna</p></div>
    <button @click="linkNumberChange(0)">glowna</button>
    <button @click="linkNumberChange(1)">kontakt</button> -->
    <div class="link" @click="linkNumberChange(0)"><p>Główna</p></div>
    <div class="link" @click="linkNumberChange(1)"><p>Informacje</p></div>
    <div class="link" @click="linkNumberChange(2)"><p>Galeria</p></div>
    <div class="link" @click="linkNumberChange(3)"><p>Historia</p></div>
    <div class="link" @click="linkNumberChange(4)"><p>kontakt</p></div>
  </div>
</div>

</template>

<script>
export default {
  data(){
    return{
      linkNumber: 0
    }
  },
  methods:{
    linkNumberChange(number){
      this.$emit('changeSite', number)
    }
  }
}
</script>
<style scoped lang="css" >
  @import ".././styles/headerStyles.css";
</style>

