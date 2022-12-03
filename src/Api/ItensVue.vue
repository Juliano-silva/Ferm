<template>
  <div id="ItemCorpo">
      <span >
          <h1 id="TitleCyber">{{book.id}}.{{book.title}}</h1>
          <img id="ImageItem" :src="book.image" alt="">
          <p id="Descrição">{{book.Descri}}</p>
          <i id="Editar" class="Editar" @click="$emit('edit-book-item', book.id)"><img src="../Arquivos/editar.png" alt=""></i>
          <i id="Apagar" class="Apagar" @click="$emit('del-book-item', book.id)"><img src="../Arquivos/excluir.png" alt=""></i>
      </span>
      <br>
  </div>
</template>
<script>
  export default{
      name: "ItensVue",
      props: ["book"]
  }
</script>
