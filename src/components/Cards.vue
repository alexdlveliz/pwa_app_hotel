<template>
    <div id="categorias" class="text-center">
      <div class="container">
        <div class="row">
          <div class="four columns cat">
            <h4>Habitaciones</h4>
          </div>
          <div class="four columns cat">
            <h4>Restaurantes</h4>
          </div>
          <div class="four columns cat">
            <h4>Comida</h4>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
    name: 'Cards'
}
</script>

<style scoped>
    #categorias{
        height: auto;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    #categorias .container{
        margin: 35px 0;
        width: 100%;
        height: auto;
    }
    #categorias .container .row{
        height: auto;
    }
    #categorias .container .row .cat{
        height: 350px;
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    #categorias .container .row .cat h4{
        padding: 10px 35px;
        background-color: var(--gradientbanner);
        backdrop-filter: blur(10px);
        font-family: var(--fontcontent);
        font-size: 22px;
        font-weight: bold;
    }
    #categorias .container .row .cat:nth-child(1){
        background-image: url(../assets/img/fondo1.jpg);
    }
    #categorias .container .row .cat:nth-child(2){
        background-image: url(../assets/img/fondo2.jpg);
    }
    #categorias .container .row .cat:nth-child(3){
        background-image: url(../assets/img/fondo4.jpg);
    }
</style>