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
      
      
        <div class="el box-4 link" id="contact" >
            <div class="contactWindow"  @click="contactShowF(true)">
                <img src="~/assets/montaz-klimatyzacji-split.jpg">
                <div class="sampleText boxText4">
                <h2>Kontakt</h2>
                <p>{{contactText}}</p>
                </div>
            </div>
            <div >
                <div class="contactInfo"  @click="contactShowF(false)">
                    <p>Email: tomasz.miga@gmail.com</p>
                    <p>Telefon: +48 123321123</p>
                    <p>ul.Chojnicka 19 Szczecinek 78-400</p>
                </div>
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
        contactShow: false,
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
    },
    contactShowF(show){
        this.contactShow = show;
    }
  }
}
</script>

<style>
  @import "~/styles/mainStyles.css";
</style>