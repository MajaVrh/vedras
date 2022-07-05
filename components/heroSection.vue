<template>
  <div>
    <div class="heroSection">
      <div class="navLinks">
        <li v-if="hr" class="hide"><b>Kontaktirajte nas</b></li>
        <li v-if="en" class="hide"><b>Contact us</b></li>
        <li>
          <a class="link" style="color: white" href="mailto:info@vedras.hr"
            >info@vedras.hr
          </a>
        </li>
        <li>
          <a class="link" style="color: white" href="tel:385989608920">
            +385 98 9608 920</a
          >
        </li>
        <li class="changeLang">
          <NuxtLink v-if="hr" to="/en"><b>EN</b> </NuxtLink>
          <NuxtLink v-if="en" to="/"><b>HR</b> </NuxtLink>
        </li>
      </div>
      <div class="logoSection">
        <img class="logo" src="@/static/Group 4.svg" alt="" />
        <hr />
      </div>

      <div class="onHold animacijaCSS">ON HOLD</div>
      <div class="iconLinks">
        <a href="https://www.instagram.com/vedrasgroup/?hl=en" target="_blank">
          <font-awesome-icon class="icon" :icon="['fab', 'instagram']"
        /></a>
        <a href="https://www.facebook.com/vedrasevents/" target="_blank"
          ><font-awesome-icon class="icon" :icon="['fab', 'facebook-f']"
        /></a>
        <a
          href="https://www.linkedin.com/uas/login?session_redirect=%2Fcompany%2F42940956%2F"
          target="_blank"
        >
          <font-awesome-icon class="icon" :icon="['fab', 'linkedin-in']"
        /></a>
      </div>
    </div>
  </div>
</template>

<script>
import { library, config } from "@fortawesome/fontawesome-svg-core";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { fab } from "@fortawesome/free-brands-svg-icons";

// This is important, we are going to let Nuxt.js worry about the CSS
config.autoAddCss = false;

// You can add your icons directly in this plugin. See other examples for how you
// can add other styles or just individual icons.
library.add(fab);
export default {
  components: { FontAwesomeIcon },
  data: () => ({
    hr: false,
    en: false,
  }),
  props: ["eng"],

  methods: {
    postaviJezik() {
      if (this.eng == true) {
        this.en = true;
      } else this.hr = true;
    },
  },
  mounted() {
    this.postaviJezik();
  },
};
</script>

<style scoped>
.navLinks {
  display: flex;
  flex-direction: row;
  gap: 8px;
  color: white;
  justify-content: flex-end;
  text-decoration: none;
  margin-right: 10% !important;
  font-size: 16px;
  letter-spacing: -0.29px;
  width: 100%;
  margin-top: 10px;
}

.logoSection {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin-right: auto;
  margin-left: auto;

  z-index: 9999;
}
.logo {
  height: 18%;

  justify-content: center;
  align-items: center;
  margin: 0 auto;
  margin-top: 8px;
  margin-bottom: 25px;
}

a {
  text-decoration: none;
  color: white;
}

hr {
  background-color: white;
  width: 437px;
  margin: 5px auto;
  padding: 0.2px;
}

.navLinks li {
  list-style: none;
}

.onHold {
  font-size: 36px;
  font-weight: 700;
  line-height: 48px;
  display: flex;
  margin: 0 auto;
  margin-top: 24px;
  color: white;
  width: 100%;
  justify-content: center;
}
.imageNav {
  width: 100%;
  object-fit: cover;
  height: 347px;
  position: relative;
  z-index: -1;
}

.heroSection {
  height: 320px;
  background-position-x: 50%;
  background-image: url("@/static/Group 6.jpg");
  background-size: cover;
  padding-top: 30px;
}

.iconLinks {
  display: flex;
  flex-direction: row;
  gap: 16px;
  margin-top: 10px;
  justify-content: center;
}
.icon {
  color: rgb(0, 0, 0);
  height: 14px;
  width: 14px;
  padding: 3px;
  background-color: rgb(255, 255, 255);
  border-radius: 100%;
  z-index: 9999;
}

@media only screen and (max-width: 700px) {
  .hide {
    display: none;
  }
  hr {
    width: 85%;
  }
  .changeLang {
    margin-left: 30px !important;
    margin-right: 20px !important;
    font-size: 16px !important;
  }
}
.changeLang {
  margin-left: 50px;
  margin-right: 10%;
  margin-bottom: 8px;
}

.link:hover {
  text-decoration: underline;
}

.animacijaCSS {
  animation-name: animacija;
  animation-duration: 1s;
  animation-direction: normal;
  animation-timing-function: ease-in;
}

@keyframes animacija {
  0% {
    opacity: 0;
    transform: translateY(10%);
    transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
