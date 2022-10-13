<template>
  <header>
    <div class="header"></div>
    <span class="pessoasproc">Os melhores filmes</span>
    <div class="logo">
      <a href="">
        <span class="fontlogo">braflix</span>
      </a>
    </div>
    <div class="submit-line">
      <input type="text" placeholder="Pesquisar Filmes" />
      <button class="submit-lente" type="submit">
        <i class="fa fa-search"></i>
      </button>
    </div>
  </header>
</template>

<style>
* {
  padding: 0;
  margin: 0;
}
a {
  text-decoration: none;
}
.submit-lente {
  position: absolute;
  top: 6px;
  right: 0;
  z-index: 10;
  border: none;
  outline: none;
}

.submit-line {
  position: relative;
  width: 200px;
}

.submit-line input {
  padding: 3px;
  width: 100%;
}

.fontlogo {
  color: #1db954;
  font-size: 2.4em;
  font-family: "Arial Black", sans-serif, Arial, Helvetica;
  font-weight: bolder;
}
header span {
  padding: 0 480px;
}
.pessoasproc {
  padding: 0;
  cursor: pointer;
}
.pesquisa input {
  padding: 3px;
  outline: none;
}
header {
  background-color: #212121;
  box-shadow: 0 0 40px 0 #1db954;
  height: 25%;
  font-size: 1.5rem;
  color: white;
  display: flex;
  align-items: center;
  font-size: 30px;
  justify-content: center;
}
.views {
  margin: 0 auto;
}
</style>
