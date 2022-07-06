<template>
  <div>
    <div>
      <heroSection :eng="eng" />
    </div>
    <div class="container-hr backgroundWhite">
      <div class="animacija">
        <div class="textMargin container-hr-col-1">
          U jeku trenutne situacije sa Co-vid19, naša je “event” branša potpuno
          zaustavljena. Zaista teško predviđamo početak velikih okupljanja i
          zabava kave priliče ljetu na kakvog smo navikli. Unatoč privremenoj
          stanci cijele event industrije, Vedras ne želi stajati po strani i
          čekati da se ova pandemija sama od sebe završi, već smo kao što to
          uvijek činimo, krenuli u nove pothvate i pobjede. Ovoga puta
          predstavljamo nešto sasvim novo, nešto što nije povezano sa našim
          uobičajenim poslovanjem. Predstavljamo nešto što će nam pomoći u borbi
          protiv ove pandemije i učiniti da se svi što prije vratimo normalnom
          životu.
        </div>
        <img
          class="marginTop UVDrobots"
          src="UVD-Robots-logo-tagline-black-website.png"
          alt=""
        />
        <img
          class="marginTop bostonMedical"
          src="boston-medical-logo-color-jpg.png"
          alt=""
        />
        <div class="marginTop text-2">
          Vedras d.o.o. Vas ovim putem želi informirati o dostupnosti autonomnog
          UV-dezinfekcijskog robota tvrtke Blue Ocean Robotics.
        </div>
      </div>
      <div>
        <img class="strojImg" src="kill-stroj.png" alt="" />
        <div class="strojTextBlock">UBIJA 99,99% MIKROORGANIZAMA</div>
      </div>
    </div>

    <div class="container-hr-2 backgroundBlue">
      <div class="NovoUPonudi" style="padding-right: 80px">
        <div class="title">Novo u našoj ponudi!</div>
        <div style="margin-top: 30px">
          Robotska dezinfekcija i sterilizacija prostora s primjenom u:
        </div>
        <div>
          <b>
            <ul class="list">
              <li>
                Turizmu (hoteli, apartmani, kuće za odmor, mobilne kućice...)
              </li>
              <li>Industriji (tvornice, skladišta, pogoni...)</li>
              <li>
                Javnim mjestima (domovi zdravlja, vrtići, škole, fakulteti,
                uredi, zračne luke, kolodvori, fitness dvorane, šoping
                centri...)
              </li>
            </ul>
          </b>
        </div>

        <div class="marginTop">
          Roboti konstruirani za čišćenje operacijskih sala i laboratorija, sada
          dezinficiraju vaše poslovne i privatne prostore.
        </div>
        <a
          target="_blank"
          style="color: white"
          href="https://uvd.blue-ocean-robotics.com"
          ><div class="marginTop link"><b>Više detalja o UVD Robots</b></div></a
        >
      </div>
      <div><img class="offerImg" loading="lazy" src="offer.png" alt="" /></div>
    </div>

    <div class="container-hr-3 backgroundWhite">
      <div class="covidFreeImgSpace">
        <img
          class="covidImg"
          loading="lazy"
          src="1_9JdjVS0SJanGma8Nt63dGw (1).jpg"
          alt=""
        />
      </div>

      <div class="covidFree animacija">
        <div class="poravnanja">
          <div class="title">#covidfree</div>
          <div style="margin-top: 20px">
            Primjenom Ultraljubičastog svjetla, (ultravioletnog, UV-c),
            UVD-robot uništava strukturu DNA u svim mikroorganizmima.
          </div>
          <div class="marginTop">
            Pružamo uslugu čišćenja velikih i malih prostora, uz pomoć robota,
            koji u najkraćem mogućem roku i autonomno dezinficiraju zatvorene
            prostore gdje sigurnost i “osjećaj čistoće” mora biti na prvom
            mjestu.
          </div>
        </div>
      </div>
    </div>
    <div class="container-hr-4">
      <img
        class="container-hr-4-img"
        src="
      Group 7.jpg"
        alt=""
      />

      <div class="backgroundBlue container-hr-4-text">
        <div class="container-hr-4-text-poravnanje">
          Želite vašim klijentima i zaposlenicima pružiti potpuno čist prostor?
          Kontaktirajte nas odmah, neka vaš prostor bude #covidfree!
        </div>
      </div>
    </div>
    <div class="container-hr-5 backgroundWhite">
      <div class="container-hr-5-text animacija">
        <div class="container-hr-5-text-poravnanje">
          <div class="title-5">
            Naše tehničko osoblje spremno je u najkraćem mogućem roku izvršiti
            uslugu koja uključuje:
          </div>

          <ul class="margin-ul-5">
            <li>dopremu UV-dezinfekcijskog robota</li>
            <li>mapiranje prostorija predviđenih za dezinfekciju</li>
            <li>kontrolu rada tijekom dezinfekcije</li>
            <li>otpremu UV-dezinfekcijskog robotas</li>
          </ul>
          <a
            target="_blank"
            href="http://vedras.hr/download/Vedras_dezinfekcija_UVD_Robotima.pdf"
            ><button class="button-5">PREUZMI BROŠURU</button></a
          >
        </div>
      </div>
      <img
        class="container-hr-5-img animacija"
        src="91448396_10158792383403455_4586978351473754112_n-1 (1).jpg"
        alt=""
      />
    </div>
    <div class="footer backgroundBlue">
      <div>Za više informacija pišite nam na mail:</div>
      <div class="footerRow animacija">
        <div class="link">
          <a style="color: white" href="mailto:info@vedras.hr"
            ><b>info@vedras.hr </b></a
          >
        </div>
        <div style="padding: 0 10px">ili nazovite broj</div>
        <div class="link">
          <a style="color: white" href="tel:385989608920"
            ><b> +385 98 9608 920</b></a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data: () => ({
    eng: false,
  }),
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Titillium+Web:ital,wght@0,200;0,300;0,400;0,600;0,700;0,900;1,200;1,300;1,400;1,600;1,700&display=swap");
body {
  font-family: "Titillium Web", sans-serif;
}
* {
  margin: 0;
  padding: 0;
}

.title {
  font-size: 36px;
  font-weight: 700;
  margin-bottom: 10px;
}

.bostonMedical {
  width: 60%;
}

.strojTextBlock {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 276px;
  height: 176px;
  color: white;
  font-size: 24px;
  padding: 0 30px;
  background-color: #027fc1;
  font-weight: bold;
  letter-spacing: -0.43px;
  line-height: 36px;
  margin-top: -20%;
}

.NovoUPonudi {
  padding-right: 125px !important;
  align-self: center;
  line-height: 32px;
  letter-spacing: -0.29px;
}

ul {
  padding-left: 20px;
}

.strojImg {
  margin-top: -40px;
  z-index: 9999;
  width: 100%;
}

.backgroundBlue {
  background-color: #027fc1;
  color: white;
}

.backgroundWhite {
  background-color: white;
  color: #5c5c5c;
}

.container-hr {
  transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
  padding: 80px 10vw;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}

.marginTop {
  margin-top: 30px;
}

.offerImg {
  height: 574px;
  width: 42.96vw;
  transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
  object-fit: cover;
}

.container-hr-2 {
  padding: 80px 80px 80px 10vw;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}
.text-2 {
  width: 73%;
}

.container-hr-3 {
  display: grid;
  padding: 160px 10vw;
  grid-template-columns: repeat(2, 1fr);
  transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
  align-items: center;
  letter-spacing: -0.29px;
}

.covidFree {
  margin-left: -0.5%;
  box-shadow: 0 2px 32px 0 rgb(0 0 0 / 14%);
  height: 464px;
}
.covidImg {
  width: 99.5%;
  height: 100%;
  object-fit: cover;
  transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
}

.covidFreeImgSpace {
  background-size: cover;
  height: 464px;
  margin-right: 20px;
}

.poravnanja {
  height: 100%;
  padding: 0px 80px;
  display: flex;
  flex-direction: column;

  justify-content: center !important;
}

.container-hr-4 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  letter-spacing: -0.64px;
  line-height: 55px;
  font-size: 36px;
}
.container-hr-4-text {
  width: 100%;

  height: 631px;
  font-size: 36px;
  font-weight: 700;
}
.container-hr-4-img {
  width: 100%;
  height: 631px;
  object-fit: cover;
}

.container-hr-4-text-poravnanje {
  padding: 0px 100px;
  height: 100%;
  display: flex;
  align-items: center;
}

.container-hr-5 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  padding: 120px 10vw;
  justify-content: space-between;
}

.container-hr-5-img {
  height: 64.26vh;
  width: 30.21vw;
  margin-left: auto;
  object-fit: cover !important;
  transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
}
.container-hr-5-text {
  box-shadow: 0 2px 32px 0 rgb(0 0 0 / 14%);
  width: 39vw;
  height: 64.26vh;
  margin-right: 80px;
  transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
}
.container-hr-5-text-poravnanje {
  padding: 0 50px;
  display: flex;
  height: 100%;
  flex-direction: column;
  justify-content: center !important;
}

.button-5 {
  height: 57px;
  width: 216px;
  font-size: 16px;
  letter-spacing: -0.29px;
  line-height: 36px;
  border: #027fc1;
  background-color: #027fc1;
  color: #fff;
}
.title-5 {
  line-height: 50px;
  font-size: 36px;
  font-weight: 700;
}
.margin-ul-5 {
  padding: 30px 0 50px 20px;
}

.footer {
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  padding: 120px 10vw;
  color: #fff;
  font-size: 36px;
  line-height: 48px;
  text-align: center;
}
.footerRow {
  display: flex !important;
  flex-direction: row;
  width: 100%;
  justify-content: center;
}

.button-5:hover {
  background-color: #fff;
  color: #027fc1;
  border: 1px solid #027fc1;
  cursor: pointer;
}

a {
  text-decoration: none;
}

.link:hover {
  text-decoration: underline;
  color: #fff;
  cursor: pointer;
}

@media (max-width: 1210px) {
  .container-hr-col-1 {
    margin-right: 5%;
  }
  .strojImg {
    margin-top: 40%;
  }
  .container-hr-5 {
    grid-template-columns: repeat(1, 1fr);
  }
  .container-hr-5-img {
    margin-top: 50px !important;
    margin: auto;
  }
  .container-hr-5-text {
    width: 90%;
    margin: auto !important;
    height: 64.26vh;
    margin-right: 80px;
  }
}
@media (max-width: 1060px) {
  .container-hr-2 {
    grid-template-columns: repeat(1, 1fr);
    padding: 80px 80px 80px 10vw !important;
  }
  .container-hr {
    padding: 80px 80px 80px 10vw !important;
  }
  .offerImg {
    height: 36.2vh;
    min-height: 300px;
    margin-top: 50px;
    width: 98%;
  }

  .text-2 {
    width: 100%;
  }
  .NovoUPonudi {
    padding-right: 0 !important;
  }
  .bostonMedical {
    width: 80% !important;
  }
  .UVDrobots {
    width: 80% !important;
  }
  .strojTextBlock {
    margin-top: -12%;
    margin-left: 0 !important;

    justify-content: flex-start !important;
  }
}

@media (max-width: 1000px) {
  .container-hr-3 {
    grid-template-columns: repeat(1, 1fr);
  }
  .container-hr-3 .covidFree:nth-of-type(2) {
    order: 1;
  }
  .container-hr-3 .covidFreeImgSpace:nth-of-type(1) {
    order: 2;
  }
  .covidFree {
    margin-left: 0;
    margin-bottom: 30px;
    height: auto;

    padding: 50px 0px;
  }
  .covidFreeImgSpace {
    height: 317px;
    width: 100%;
  }
}
@media (max-width: 1010px) {
  .container-hr-4 {
    grid-template-columns: repeat(1, 1fr);
  }
  .container-hr-4 .container-hr-4-img:nth-of-type(1) {
    order: 2;
  }
  .container-hr-4 .container-hr-4-text:nth-of-type(2) {
    order: 1;
  }
  .container-hr-4-text {
    height: auto;
    padding: 50px 0px;
  }
  .container-hr-4-img {
    height: 55vh;
    min-height: 300px;
  }

  .container-hr-5-text {
    width: 100%;
    margin: auto !important;
    height: 64.26vh;
    margin-right: 80px;
  }
  .container-hr-5-img {
    width: 50%;
  }
}
@media (max-width: 850px) {
  .footerRow {
    display: block !important;
  }
}

@media (max-width: 800px) {
  .container-hr {
    grid-template-columns: repeat(1, 1fr);
    padding: 80px 25px !important;
    margin: 0px 10vw;
  }
  .container-hr-2 {
    padding: 80px 20px !important;
  }

  .strojImg {
    margin-top: 0px;
  }
  .bostonMedical {
    width: 60% !important;
  }
  .UVDrobots {
    width: 50% !important;
  }
  .textMargin {
    width: 100%;
  }
  .offerImg {
    height: 36.2vh;
    min-height: 300px;
  }
  .title {
    font-size: 24px;
  }

  .NovoUPonudi {
    line-height: 24px;
    padding-left: 20px;
  }

  .strojTextBlock {
    width: 316px !important;
    justify-content: center;
    margin-left: auto;
    margin-right: auto;
  }
}

@media (max-width: 700px) {
  .container-hr {
    grid-template-columns: repeat(1, 1fr);
    padding: 80px 0 !important;
    margin: 0px 20px;
  }

  .container-hr-3 {
    padding: 160px 20px !important;
  }
  .container-hr-4-text {
    font-size: 25px;
    line-height: 32px;
  }
  .container-hr-4-text-poravnanje {
    padding: 0px 50px;
  }
  .container-hr-5 {
    padding: 120px 20px !important;
  }

  .container-hr-5-img {
    width: 100%;
  }
  .container-hr-5-text {
    width: 100%;
    height: auto !important;
  }
  .title-5 {
    line-height: 32px;
    font-size: 25px;
  }
  .container-hr-5-text-poravnanje {
    padding: 50px 20px;
    margin: 0 !important;
  }
  .footer {
    font-size: 25px;
    line-height: 32px;
  }
}

@media (max-width: 600px) {
  .container-hr-3 {
    padding: 80px 20px !important;
  }
  .poravnanja {
    padding: 0 20px;
  }
}
@media (max-width: 400px) {
  .strojTextBlock {
    width: 83% !important;
  }
}

.animacija {
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
