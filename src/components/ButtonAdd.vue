<template>
  <div>
    <b-button class="boton-estilo-sum" pill variant="info">+</b-button>
  </div>
</template>

<script>
export default {
    name:"ButtonAdd",
    prop:{
        añadir: String,
    }

}
</script>

<style scoped>
.boton-estilo-sum {
  padding-left: 14px;
  padding-right: 14px;
  margin-left: 155%;
}
</style>