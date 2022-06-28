<template>
  <v-main class="body2" id="">
    <v-row>
      <v-col class="d-flex" cols="12" md="6">
        <div class="container-a">
          <v-img class="img" src="@/assets/perfil.jpg"></v-img>
        </div>
        <div class="container-b">
          <ul>
            <li>
              Estou estudando programação Fronte-End e Back-end no Estituto
              Federal Catarinense.
            </li>
            <li>
              Estou atuando com HTML, CSS, Javascript, Python Vue, Vue-tify e
              Firebase
            </li>
            <li>Procuro obter boas experiências em minha área.</li>
          </ul>

          <div class="logos">
            <div class="logo"><v-img src="@/assets/vue.png"></v-img></div>
            <div class="logo"><v-img src="@/assets/javas.png"></v-img></div>
          </div>
        </div>
      </v-col>

      <v-col class="ladoEs red--text text-center" cols="12" md="6"> </v-col>
    </v-row>
  </v-main>
</template>

<script>
export default {
  name: "socialMedia",
  data() {
    return {};
  },
};
</script>

<style></style>
