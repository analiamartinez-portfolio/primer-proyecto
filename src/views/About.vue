<template>
  <div>
    <b-container>
      <b-row>
        <Titulos msg="Sobre Nosotros" />
      </b-row>
      <b-row>
        <b-col cols="4" align-self="start">
          <img class="img-señor" src="../assets/imgSecundarioAbout.webp" alt="señorInteresado" />
        </b-col>
        <b-col cols="8">
          <b-row>
            <b-col>
              <p
                class="about-text"
              >Los programas ofrecen una combinación de actividades a su propio ritmo, foros de discusión colaborativos y eventos en línea en vivo dirigidos por expertos.</p>
            </b-col>
            <b-col>
              <p
                class="about-text"
              >Nuestra red de expertos de profesores, autores y líderes de opinión guían a los estudiantes a lo largo del programa.</p>
            </b-col>
          </b-row>
          <b-row>
            <img
              class="imgAboutPrincipal"
              src="../assets/imgAboutPrincipal.webp"
              alt="imgPrincipal"
            />
          </b-row>
        </b-col>
      </b-row>
      <ButtonVolver />
    </b-container>
  </div>
</template>

<script>
import Titulos from "../components/Titulos.vue";
import ButtonVolver from "../components/ButtonVolver.vue";

export default {
  name:"About",
  components: {
    Titulos,
    ButtonVolver,
  },
}
</script>

<style>
.about-text {
  text-align: left;
  font-size: 18px;
}
.img-señor {
  text-align: left;
  margin-left: -36%;
  padding-top: 15%;
}
.imgAboutPrincipal {
  padding-left: 15%;
  width: 70%;
}
</style>
