<template>
  <v-app class="d-flex">
    <v-app-bar app class="grey darken-4">
      <v-spacer></v-spacer>
      <v-btn class="btn Home mr-10" @click="$vuetify.goTo('#home')">Home</v-btn>
      <v-btn
        class="btn SocialMedia mr-10"
        @click="$vuetify.goTo('#socialMedia')"
        >Social Media</v-btn
      >
      <v-btn class="btn Projects mr-10" @click="$vuetify.goTo('#projectsMe')"
        >Projects</v-btn
      >
      <v-btn class="btn AboutMe mr-10" @click="$vuetify.goTo('#aboutMe')"
        >About me</v-btn
      >
    </v-app-bar>

    <v-main class="body" id="home">
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

    <socialMedia id="socialMedia" />
    <projectsMe id="projectsMe" />
    <aboutMee id="aboutMe" />
  </v-app>
</template>

<script>
import socialMedia from "./components/socialMedia.vue";
import projectsMe from "./components/projectsMe.vue";
import aboutMee from "./components/aboutMee.vue";
export default {
  components: { socialMedia, projectsMe, aboutMee },
  data() {
    return {};
  },
};
</script>

<style>
.body {
  background-image: url(assets/teste1.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: auto;
}
.logos {
  width: 800px;
}

.logo {
  margin-left: 24px;
  display: flex;
  height: 10%;
  width: 8%;
  display: inline-block;
}

.img {
  border-radius: 120px;
}

.container-a {
  margin-top: 40px;
  margin-left: 30px;
  display: inline-block;
  width: 30%;
  height: 30%;
}
.container-b {
  width: 70%;
  color: white;
  font-size: 20px;
  font-family: "garamond", "Helvetica Neue", "Helvetica";
  margin-top: 100px;
  margin-left: 10px;
  display: inline-block;
}

.btn,
.btn2 {
  width: 130px;
  height: 100px;
  text-align: center;
  line-height: 100px;
  color: rgba(255, 255, 255, 0.9);
  background: linear-gradient(-45deg, #e4e4e4, #a71906, #3fbce2, #21d63f);
  background-size: 600%;
  -webkit-animation: anime 16s linear infinite;
  animation: anime 16s linear infinite;
}
.btn2 {
  position: absolute;
  margin-top: -70px;
  z-index: -1;
  filter: blur(30px);
  opacity: 0.8;
}
@-webkit-keyframes anime {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
@keyframes anime {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
</style>
