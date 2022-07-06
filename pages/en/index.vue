<template>
  <div>
    <div>
      <heroSection :eng="eng" />
    </div>
    <div class="container-en backgroundWhite">
      <div class="animacija">
        <div class="textMargin container-en-col-1">
          In the midst of the current situation with Co-vid19, our “event”
          industry is completely stopped. It is really hard to predict the start
          of big gatherings and coffee parties that are close to the summer we
          are used to. Despite the temporary pause of the entire event industry,
          Vedras does not want to stand aside and wait for this pandemic to end
          on its own, but as we always do, we are embarking on new ventures and
          victories. This time around, we are introducing something completely
          new, something unrelated to our usual business. We present something
          that will help us combat this pandemic and make everyone return to
          normal as soon as possible.
        </div>
        <img
          class="marginTop UVDrobots"
          src="/UVD-Robots-logo-tagline-black-website.png"
          alt=""
        />
        <img
          class="marginTop bostonMedical"
          src="/boston-medical-logo-color-jpg.png"
          alt=""
        />
        <div class="marginTop text-2">
          We want to inform you of the availability of a new autonomous UV
          disinfection robot from the Blue Ocean Robotics company.
        </div>
      </div>
      <div>
        <img class="strojImg" src="/kill-stroj.png" alt="" />
        <div class="strojTextBlock">KILLS 99,99% OF MICROORGANISMS</div>
      </div>
    </div>

    <div class="container-en-2 backgroundBlue">
      <div class="NovoUPonudi" style="padding-right: 80px">
        <div class="title">New in our offer!</div>
        <div style="margin-top: 30px">
          Secure robot disinfection and sterilization with applications in:
        </div>
        <div>
          <b>
            <ul class="list">
              <li>
                Tourism (hotels, apartments, holiday homes, mobile homes ...)
              </li>
              <li>Industry (factories, warehouses, plants ...)</li>
              <li>
                Public places (health centers, kindergartens, schools, colleges,
                offices, airports, stations, fitness gyms, shopping centers ...)
              </li>
            </ul>
          </b>
        </div>

        <div class="marginTop">
          Robots designed to clean operating rooms and laboratories are now
          disinfecting your business and private spaces.
        </div>
        <a
          target="_blank"
          style="color: white"
          href="https://uvd.blue-ocean-robotics.com"
          ><div class="marginTop link">
            <b>More details about UVD Robots</b>
          </div></a
        >
      </div>
      <div><img class="offerImg" loading="lazy" src="/offer.png" alt="" /></div>
    </div>

    <div class="container-en-3 backgroundWhite">
      <div class="covidFreeImgSpace">
        <img
          class="covidImg"
          loading="lazy"
          src="/1_9JdjVS0SJanGma8Nt63dGw (1).jpg"
          alt=""
        />
      </div>

      <div class="covidFree animacija">
        <div class="poravnanja">
          <div class="title">#covidfree</div>
          <div style="margin-top: 20px">
            By applying ultraviolet light (UV, UV-c), the UVD robot destroys the
            structure of DNA in all microorganisms.
          </div>
          <div class="marginTop">
            With help of robots, we provide a service for cleaning large and
            small spaces, which in the shortest possible time and autonomously
            disinfect indoors where safety and “sense of cleanliness” must come
            first.
          </div>
        </div>
      </div>
    </div>
    <div class="container-en-4">
      <img class="container-en-4-img" src="/Group 7.jpg" alt="" />

      <div class="backgroundBlue container-en-4-text">
        <div class="container-en-4-text-poravnanje">
          You want to provide a secure place to stay or work for your costumers
          or employees. Search no more and contact us now. Let your spaces be
          #covidfree
        </div>
      </div>
    </div>
    <div class="container-en-5 backgroundWhite">
      <div class="container-en-5-text animacija">
        <div class="container-en-5-text-poravnanje">
          <div class="title-5">
            Our staff is ready to provide a service as soon as possible which
            includes:
          </div>

          <ul class="margin-ul-5">
            <li>delivery of UV disinfection robot</li>
            <li>mapping of the rooms intended for disinfection</li>
            <li>control of operation during disinfection</li>
            <li>collection of the UV disinfection robot</li>
          </ul>
          <a
            target="_blank"
            href="http://vedras.hr/download/Vedras_dezinfekcija_UVD_Robotima.pdf"
            ><button class="button-5">DOWNLOAD BROCHURE</button></a
          >
        </div>
      </div>
      <img
        class="container-en-5-img animacija"
        src="/91448396_10158792383403455_4586978351473754112_n-1 (1).jpg"
        alt=""
      />
    </div>
    <div class="footer backgroundBlue">
      <div>Contact us for more:</div>
      <div class="footerRow animacija">
        <div class="link">
          <a style="color: white" href="mailto:info@vedras.hr"
            ><b>info@vedras.hr </b></a
          >
        </div>
        <div style="padding: 0 10px">or call us</div>
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
    eng: true,
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

.container-en {
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

.container-en-2 {
  padding: 80px 80px 80px 10vw;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}
.text-2 {
  width: 73%;
}

.container-en-3 {
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

.container-en-4 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  letter-spacing: -0.64px;
  line-height: 55px;
  font-size: 36px;
}
.container-en-4-text {
  width: 100%;

  height: 631px;
  font-size: 36px;
  font-weight: 700;
}
.container-en-4-img {
  width: 100%;
  object-fit: cover;
  height: 631px;
}

.container-en-4-text-poravnanje {
  padding: 0px 100px;
  height: 100%;
  display: flex;
  align-items: center;
}

.container-en-5 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  padding: 120px 10vw;
  justify-content: space-between;
}

.container-en-5-img {
  height: 64.26vh;
  width: 30.21vw;
  margin-left: auto;
  object-fit: cover !important;
  transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
}
.container-en-5-text {
  box-shadow: 0 2px 32px 0 rgb(0 0 0 / 14%);
  width: 39vw;
  height: 64.26vh;
  margin-right: 80px;
  transition: all 1s cubic-bezier(0.36, 0.69, 0.3, 0.64);
}
.container-en-5-text-poravnanje {
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
  .container-en-col-1 {
    margin-right: 5%;
  }
  .strojImg {
    margin-top: 10%;
  }
  .container-en-5 {
    grid-template-columns: repeat(1, 1fr);
  }
  .container-en-5-img {
    margin-top: 50px !important;
    margin: auto;
  }
  .container-en-5-text {
    width: 90%;
    margin: auto !important;
    height: 64.26vh;
    margin-right: 80px;
  }
}
@media (max-width: 1060px) {
  .container-en-2 {
    grid-template-columns: repeat(1, 1fr);
    padding: 80px 80px 80px 10vw !important;
  }
  .container-en {
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
  .container-en-3 {
    grid-template-columns: repeat(1, 1fr);
  }
  .container-en-3 .covidFree:nth-of-type(2) {
    order: 1;
  }
  .container-en-3 .covidFreeImgSpace:nth-of-type(1) {
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
  .container-en-4 {
    grid-template-columns: repeat(1, 1fr);
  }
  .container-en-4 .container-en-4-img:nth-of-type(1) {
    order: 2;
  }
  .container-en-4 .container-en-4-text:nth-of-type(2) {
    order: 1;
  }
  .container-en-4-text {
    height: auto;
    padding: 50px 0px;
  }
  .container-en-4-img {
    height: 55vh;
    min-height: 300px;
  }

  .container-en-5-text {
    width: 100%;
    margin: auto !important;
    height: 64.26vh;
    margin-right: 80px;
  }
  .container-en-5-img {
    width: 50%;
  }
}
@media (max-width: 850px) {
  .footerRow {
    display: block !important;
  }
}

@media (max-width: 800px) {
  .container-en {
    grid-template-columns: repeat(1, 1fr);
    padding: 80px 25px !important;
    margin: 0px 10vw;
  }
  .container-en-2 {
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

  .container-en-3 {
    padding: 160px 20px !important;
  }
  .container-en-4-text {
    font-size: 25px;
    line-height: 32px;
  }
  .container-en-4-text-poravnanje {
    padding: 0px 50px;
  }
  .container-en-5 {
    padding: 120px 20px !important;
  }

  .container-en-5-img {
    width: 100%;
  }
  .container-en-5-text {
    width: 100%;
    height: auto !important;
  }
  .title-5 {
    line-height: 32px;
    font-size: 25px;
  }
  .container-en-5-text-poravnanje {
    padding: 50px 20px;
    margin: 0 !important;
  }
  .footer {
    font-size: 25px;
    line-height: 32px;
  }
}

@media (max-width: 600px) {
  .container-en-3 {
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
