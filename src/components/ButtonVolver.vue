<template>
  <div>
    <b-button @click="back" class="botonVolver" variant="outline-primary">Volver</b-button>
  </div>
</template>

<script>
export default {
    name:"ButtonVolver",
    props:{
        Volver: String,
    },

    data(){
      return{}
    },

  methods:{
    back(){
      this.$router.back()
    },
  }

}
</script>

<style scoped>
.botonVolver {
  margin-top: 3%;
  background-color: plum;
  font-size: 16px;
  color: white;
  border-color: rgb(211, 161, 211);
  font-weight: bold;
  padding-right: 24px;
  padding-left: 24px;
  margin-right: 90%;
}
</style>