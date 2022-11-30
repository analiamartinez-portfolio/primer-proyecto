<template>
  <div>
    <h1 class="title1">{{msg}}</h1>
  </div>
</template>

<script>

export default {
    name: "Titulos",
    props: {
        msg: String,
    },
};
</script>

<style scoped>
.title1 {
  text-align: left;
  margin-bottom: 5%;
}
</style>