<template>
  <div id="registro" class="text-center">
      <div class="container">
        <div class="row">
          <div class="twelve columns tit">
            <h3>Regístrate para poder enviarte más información</h3>
          </div>
        </div>
        <div class="row">
          <div class="three columns campo">
            <input type="text" name="Nombre" id="name" placeholder="Nombre" required/>
          </div>
          <div class="three columns campo">
            <input type="text" name="Apellido" id="lastname" placeholder="Apellido" required/>
          </div>
          <div class="three columns campo">
            <input type="email" name="correo" id="email" placeholder="Correo" required/>
          </div>
          <div class="three columns campo">
            <button>Regístrate</button>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
    name: 'Registro'
}
</script>

<style scoped>
    #registro{
        height: auto;
        background-color: var(--bckgreg);
        display: flex;
        justify-content: center;
        align-items: center;
    }
    #registro .container{
        min-width: 90%;
        height: auto;
    }
    #registro .container .row{
        margin: 35px 0;
    }
    #registro .container .row .tit h3{
        font-family: var(--fontsubt);
        font-size: 28px;
    }
    #registro .container .row .campo input{
        width: 100%;
        border: solid 1px var(--fontc);
        font-family: var(--fontcontent);
    }
    #registro .container .row .campo button{
        width: 100%;
        border: solid 1px var(--fontc);
    }
</style>