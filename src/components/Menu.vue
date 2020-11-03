<template>
  <div id="menu" class="text-center">
      <div class="container">
        <div class="row">
          <div class="four columns item">
            <a href="">Item</a>
          </div>
          <div class="four columns item">
            <a href="">Item</a>
          </div>
          <div class="four columns item">
            <a href="">Item</a>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
name: "Menu"
}
</script>

<style  scoped>
@import "./../assets/css/skeleton.css";
#menu {
    margin: 0;
    border-bottom: solid 2px var(--fontc);
    background-color: var(--bckgreg);
  
}
#menu .container .row .item {
    padding-top: 12px;
    padding-bottom: 12px;
}
#menu .container .row .item a {
    text-decoration: none;
    font-family: var(--fontcontent);
    color: var(--fontc);
    font-weight: 1000;
}
</style>
