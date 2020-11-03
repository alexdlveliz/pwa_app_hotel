<template>
  <div id="app">
    <header>
      <Menu></Menu>
    </header>
    <main>
      <Banner></Banner>
      <Cards></Cards>
      <Registro></Registro>
      <Photos></Photos>
      <Album></Album>
      <Footer></Footer>
    </main>
  </div>
</template>

<script>
import Menu from './components/Menu';
import Banner from './components/Banner'
import Cards from './components/Cards'
import Registro from './components/Registro'
import Photos from './components/Photos'
import Album from './components/Album'
import Footer from './components/Footer'

export default {
  name: 'app',
  components: {
    Menu,
    Banner,
    Cards,
    Registro,
    Photos,
    Album,
    Footer
  }
}
</script>

<style>
:root{
  
  --bckg: #fdf9f6;
  --bckgnav: #e9e9e9;
  --bckgreg: #e36414;
  --bckglog: #fdf9f7;
  --fontc: #001233;
  --fontcnav: #fdf9f7;
  --gradientbanner: rgba(255, 255, 255, 0.6);

  --fontt2: 'Playfair Display', serif;
  --fonttsubt: 'PT Sans', sans-serif;
  /* --fontcontent: "helvetica"; */
  --fontcontent: 'Lora', serif;
}

body {
  margin: 0;
  padding: 0;
}
header{
  margin: 0;
  padding: 0;
}
.text-center {
  text-align: center;
}


</style>
