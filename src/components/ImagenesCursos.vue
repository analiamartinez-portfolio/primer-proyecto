<template>
  <div>
    <b-img :src="srcImg" fluid alt="Responsive image" />
    <b-row class="añadir-espacios">
      <b-col cols="1">
        <b-button @click="sum" class="boton-estilo" pill variant="info">+</b-button>
      </b-col>
      <b-col cols="1">
        <b-button @click="rest" class="boton-estilos" pill variant="info">-</b-button>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
    name:"ImagenesCursos",
    props:{
       srcImg: String,
    },
    data(){
        return{
        }
    },
    methods: {
       rest(){
         this.$emit('restar')
       },
       sum(){
         this.$emit('sumar')
       }
    }
}
</script>

<style scoped>
.boton-estilos {
  padding-left: 16px;
  padding-right: 16px;
}
.boton-estilo {
  padding-left: 14px;
  padding-right: 14px;
  /* margin-left: 165%; */
}
.añadir-espacios {
  padding-top: 3%;
  padding-bottom: 15%;
}
</style>