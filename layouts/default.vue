<template>
  <div id="container" >
    <!-- <app-header /> -->
    <div class="nuxt-container"><Nuxt/></div>
    <!-- <app-footer /> -->
  </div>
  
</template>
<script>
import AppHeader from '~/components/appHeader'
import AppFooter from '~/components/appFooter'

export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<style>


#__nuxt, #__layout, #container {
  height: 100%;
    box-sizing: border-box;

}
#container {
  /*
  display: flex;
  flex-direction: column;
*/
  box-sizing: border-box;

}
.nuxt-container {
  height: calc(100% - 70px); /* value in px is navHeight */
  flex: 1;
  box-sizing: border-box;

}
body{
  height: 100%;
  box-sizing: border-box;

}
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  height: 100%;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
