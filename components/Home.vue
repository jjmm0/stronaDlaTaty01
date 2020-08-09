<template>
  <div class="wrapper"> 
      <div class="grid">
        <div class="el box-1" id="main">
          <img src="~/assets/montaż-maszyn.jpg">
          <div class="sampleText boxText1">
            <h2>Strona główna</h2>
            <p>{{mainText}}</p>
          </div>
        </div>
        <div class="el box-2 link" id="info" @click="linkNumberChange(1)">
            <img src="~/assets/Relokacja-maszyn-co-to-znaczy-1024x536.jpg">
            <div class="sampleText boxText2">
              <h2>Informacje</h2>
              <p>{{infoText}}</p>
            </div>    
        </div>
      
        <div class="el box-3 link" id="gallery" @click="linkNumberChange(2)">
            <img src="~/assets/13-44.jpg">
            <div class="sampleText boxText3">
              <h2>Galeria</h2>
              <p>{{galleryText}}</p>
            </div>
        </div>
      
      
        <div class="el box-4 link" id="contact" @click="linkNumberChange(4)">
            <img src="~/assets/montaz-klimatyzacji-split.jpg">
            <div class="sampleText boxText4">
              <h2>Kontakt</h2>
            <p>{{contactText}}</p>
            </div>
          
        </div>
      
      
        <div class="el box-5 link" id="history" @click="linkNumberChange(3)">
            <img src="~/assets/schemat.jpg">
            <div class="sampleText boxText5">
              <h2>Ostatnie zlecenia</h2>
            <p>{{historyText}}</p>
            </div>
        </div>
      </div>
      
  </div>
</template>

<script>

export default {
  data(){
    return{
      mainText: '1Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Mattis vulputate enim nulla aliquet porttitor lacus luctus accumsan. Tortor aliquam nulla facilisi cras.',
      infoText: 'Kliknij, aby dowiedzieć się więcej...',
      galleryText: 'Kliknij, aby dowiedzieć się więcej...',
      contactText: 'Kliknij, aby dowiedzieć się więcej...',
      historyText: 'Kliknij, aby dowiedzieć się więcej...',
    }
  },
    methods:{
    linkNumberChange(number){
      this.$emit('changeSite', number)
    }
  }
}
</script>

<style>
  @import "~/styles/mainStyles.css";
</style>