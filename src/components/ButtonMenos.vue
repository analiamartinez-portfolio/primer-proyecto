<template>
  <div>
    <b-button class="boton-estilos" pill variant="info">-</b-button>
  </div>
</template>

<script>
export default {
    name:"ButtonMenos",
    prop:{
        quitar: String,
    }
}
</script>

<style scoped>
.boton-estilos {
  padding-left: 16px;
  padding-right: 16px;
  margin-left: 70%;
}
</style>