<template>
  <div class="wrapper"> 
      <div class="grid">
        <div class="el box-1" id="main">
          <img src="..\images\montaż-maszyn.jpg">
          <div class="sampleText boxText1">
            <h2>Strona główna</h2>
            <p>{{box1Text}}</p>
          </div>
        </div>
        <div class="el box-2" id="info">
          <a href="./info">
            <img src="..\images\Relokacja-maszyn-co-to-znaczy-1024x536.jpg">
            <div class="sampleText boxText2">
              <h2>Informacje</h2>
              <p>{{box2Text}}</p>
            </div>    
          </a> 
        </div>
      
        <div class="el box-3" id="gallery">
          <a href="./gallery">
            <img src="..\images\13-44.jpg">
            <div class="sampleText boxText3">
              <h2>Galeria</h2>
              <p>{{box3Text}}</p>
            </div>
          </a>
        </div>
      
      
        <div class="el box-4" id="contact">
          <a href="./contact">
            <img src="..\images\montaz-klimatyzacji-split.jpg">
            <div class="sampleText boxText4">
              <h2>Kontakt</h2>
            <p>{{box4Text}}</p>
            </div>
          </a>
        </div>
      
      
        <div class="el box-5" id="history">
          <a href="./history">
            <img src="..\images\schemat.jpg">
            <div class="sampleText boxText5">
              <h2>Ostatnie zlecenia</h2>
            <p>{{box5Text}}</p>
            </div>
          </a>
        </div>
      </div>
      
  </div>
</template>

<script>

export default {
  data(){
    return{
      box1Text: '1Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Mattis vulputate enim nulla aliquet porttitor lacus luctus accumsan. Tortor aliquam nulla facilisi cras.',
      box2Text: '2Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
      box3Text: '3Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
      box4Text: '4Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
      box5Text: '5Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
    }
  }
}
</script>

<style>
  @import ".././styles/mainStyles.css";
</style>