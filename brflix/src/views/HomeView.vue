<script setup></script>

<template>
  <div class="bemvindo">
    <span>Os melhores filmes estão aqui</span>
    <router-link to="/list">
      <button class="btnenter">Acesse a lista</button>
    </router-link>
  </div>
</template>
<style>
body {
  background-color: #212121;
}

.bemvindo {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: white;
  font-size: 1.8rem;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: bold;
  margin-top: 27%;
  padding: 20px;
}

.bemvindo button {
  padding: 15px;
  border-radius: 25px;
  text-decoration: none;
  border: none;
  min-width: 140px;
  cursor: pointer;
  background-color: #1db954;
  margin-top: 15px;
}
.btnenter a {
  color: #1db954;
}
</style>
