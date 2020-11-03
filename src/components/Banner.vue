<template>
  <div id="banner" class="text-center">
    <div class="container">
      <div class="row">
        <div class="twelve columns bann">
          <h1>Hotel 5 estrellas</h1>
          <p>
            Cupcake ipsum dolor sit amet marzipan. Chocolate cake dessert icing
            cotton candy. Pudding brownie tiramisu soufflé sweet jujubes lemon
            drops tootsie roll. Sweet roll pastry cookie gummies gummies
            gingerbread cake fruitcake. Apple pie candy canes brownie icing.
            Lollipop pastry cake powder powder. Danish danish chocolate pudding
            marshmallow candy canes cotton candy. Carrot cake icing apple pie.
            Gummies cookie chocolate bar tootsie roll bear claw. Danish pudding
            icing oat cake.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style scoped>
#banner {
  height: auto;
  background-image: url(../assets/img/fheader.jpg);
  background-position: center;
  background-size: cover;
  background-repeat: repeat;
  background-attachment: fixed;
  display: flex;
  align-items: center;
  justify-content: center;
}

#banner .container {
  margin: 80px 0;
  height: auto;
  background-color: var(--gradientbanner);
  backdrop-filter: blur(6px);
  border-radius: 10px;
}

#banner .container .row {
  height: auto;
}

#banner .container .row .bann {
  height: auto;
}

#banner .container .row .bann h1 {
  margin-top: 10px;
  font-family: var(--fontt2);
}

#banner .container .row .bann p {
  margin: 20px;
  padding: 35px;
  border: solid 1px var(--fontc);
  font-family: var(--fontcontent);
  font-size: 13px;
}
</style>