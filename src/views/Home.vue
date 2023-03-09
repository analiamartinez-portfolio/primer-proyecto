<template>
  <div class="home">
    <b-container>
      <b-row align-v="center">
        <b-col>
          <img src="../assets/imgUdemyHome.jpeg" alt="imgHome" />
        </b-col>
      </b-row>

      <b-row class="spaces" align-v="center">
        <b-col>
          <h1>Una amplia selección de cursos</h1>
        </b-col>
      </b-row>

      <b-row align-v="center">
        <b-col>
          <p>Elige entre 204.000 cursos de vídeo en línea con nuevo contenido cada mes</p>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: "Home",
  components: {
  
  },
};
</script>

<style scoped>
.spaces {
  padding-top: 7%;
  padding-bottom: 1%;
}
</style>
