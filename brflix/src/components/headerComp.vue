<template>
  <header>
    <div class="header"></div>
    <span class="pessoasproc">Os melhores filmes</span>
    <div class="logo">
      <a href="">
        <span class="fontlogo">B R A F L I X</span>
      </a>
    </div>
    <div class="submit-line">
      <img src="../img/6063509.png" alt="">
    </div>
  </header>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
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
.submit-line img {
  width: 20%;
}

.submit-line input {
  padding: 3px;
  width: 100%;
}

.fontlogo {
  color: #1db954;
  font-size: 2em;
  font-family: "Poppins";
  font-weight: 600;
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
  box-shadow: 0 0 40px 0 #1db95460;
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
