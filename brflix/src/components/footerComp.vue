<template>

    <div class="bemvindo">
    <span>Os melhores filmes estão aqui</span>
    <router-link to="/list">
    <button class="btnenter">
      Acesse a lista
    </button>
</router-link>
  </div>
</template>
<style>
    .bemvindo {
    background-color: #0a0a12;
    padding: 0 20px;
    bottom: 0;
    position: fixed;
    width: 100%;
}
.txtprin{
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 1.5%;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: bold;
    color: white;
    font-size: 2em;
    margin-right: 14.5%;
}

.categorias{
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
}
.btnenter{
    color: #fff;
}
.categorias span{
    margin: 0 4%;
}
</style>