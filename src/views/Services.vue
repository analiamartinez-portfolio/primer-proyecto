<template>
  <div>
    <b-container class="aprovechar-espacios">
      <b-row>
        <b-col>
          <Titulos msg="Nuestros servicios" />
        </b-col>
        <b-col>
          <b-input v-model="total" type="number"></b-input>
        </b-col>
      </b-row>
      <b-row>
        <b-col cols="6" v-for="image in images" :key="image.index">
          <ImagenesCursos :srcImg="image.src" @restar="rest" @sumar="sum" />
        </b-col>
        <b-row>
          <b-col>
            <ButtonVolver />
          </b-col>
          <b-col>
            <b-button @click="addOrDelete(isVisible)" class="button-gratis">Gratis</b-button>
          </b-col>
        </b-row>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Titulos from "../components/Titulos.vue";
import ButtonVolver from "../components/ButtonVolver.vue";
import ImagenesCursos from "../components/ImagenesCursos.vue";

export default {
  name: "Services",
 components: {
    Titulos,
    ButtonVolver,
    ImagenesCursos,
  },
  data(){
        return{
          isVisible: true,
          total:0,
          images:[
            {
            src:"https://edteam-media.s3.amazonaws.com/courses/original/3886d909-4c3a-4e5c-a004-68cc5fcdccea.png"
            },
            {
              src:"https://edteam-media.s3.amazonaws.com/courses/original/ac16bf26-6b10-4065-b729-ebb008933936.png"
            },
            {
            src:"https://ed.team/_next/image?url=https%3A%2F%2Fedteam-media.s3.amazonaws.com%2Fcourses%2Fbig%2F9ccf39c6-3e21-411d-9f09-c3589cf93750.png&w=1920&q=75"
            },
            {
              src:"https://ed.team/_next/image?url=https%3A%2F%2Fedteam-media.s3.amazonaws.com%2Fcourses%2Fbig%2F9fc241a3-128a-413f-936a-75b2e54b233f.jpg&w=1920&q=75"
            },
            {
              src:"https://ed.team/_next/image?url=https%3A%2F%2Fedteam-media.s3.amazonaws.com%2Fcourses%2Fbig%2F1fc49db5-2454-43e5-b94b-bed0d98719f2.png&w=1920&q=75"
            },
            {
              src:"https://ed.team/_next/image?url=https%3A%2F%2Fedteam-media.s3.amazonaws.com%2Fcourses%2Fbig%2F82daef93-44b7-4a0a-9910-42aa609c6eee.png&w=1920&q=75"
            },
          ]
        }
    },
    methods: {
      addOrDelete(visible){
           visible ? this.isVisible = false : this.isVisible = true
      },
      rest(){
        this.total--;
      },
      sum(){
        this.total++;
      }
},
}
</script>

<style scoped>
.espacios {
  padding-top: 3%;
}
.button-gratis {
  margin-top: 3%;
  background-color: rgb(117, 117, 243);
  font-size: 16px;
  color: white;
  border-color: rgb(133, 135, 233);
  font-weight: bold;
  padding-right: 24px;
  padding-left: 24px;
  margin-left: 83%;
}
.aprovechar-espacios {
  padding-bottom: 8%;
}
</style>