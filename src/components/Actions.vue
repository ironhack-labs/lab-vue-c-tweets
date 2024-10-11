# componente será responsable de mostrar los botones de interacción del tweet 
<template>
    <div class="actions">
        <button><i class="fas fa-comment"></i></button>
      <button><i class="fas fa-retweet"></i></button>
      <button><i class="fas fa-heart"></i></button>
      <button><i class="fas fa-share"></i></button>
      </div>
  </template>
  
  <style scoped>
  .actions {
    display: flex;
    justify-content: space-around;
    margin-top: 10px;
  }
  button {
    background: none;
    border: none;
    cursor: pointer;
    font-size: 1.2em;
  }
  </style>
  