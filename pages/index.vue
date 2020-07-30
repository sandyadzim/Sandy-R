<template>
  <div
    class="container-fluid"
    style="padding-left: 0px !important; padding-right: 0px !important;"
  >
    <!-- ================ HOME ================ -->
    <section id="home" class="site-home">
      <div class="container">
        <div class="row">
          <div class="col-lg-6 col-md-12 site-title">
            <h1 class="font-weight-bold">Hallo,</h1>
            <h3>Perkenalkan saya</h3>
            <h1 class="font-weight-bold">Sandy Rahmansyah</h1>
            <h5 class="font-weight-bold"><em>Front End Developer</em></h5>
            <div class="site-buttons">
              <div>
                <a
                  href="https://api.whatsapp.com/send?phone=6283153440780"
                  target="_blank"
                >
                  <button class="btn-custom color-btn-wa mr-4">
                    WhatsApp
                  </button>
                </a>
                <a
                  href="https://mail.google.com/mail/?view=cm&fs=1&to=sandy.adzim@gmail.com"
                  target="_blank"
                >
                  <button class="btn-custom color-btn-email">
                    Email
                  </button>
                </a>
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-md-6 banner-image">
            <img
              src="../assets/img/sandy-banner.svg"
              alt="banner-img"
              class="img-fluid"
            />
          </div>
        </div>
      </div>
    </section>
    <!-- ================ End HOME ================ -->
    <!-- ================ ABOUT ================= -->
    <section id="about" class="site-about">
      <div class="container-fluid">
        <div class="row">
          <div class="col-lg-6 col-md-12">
            <img
              src="../assets/img/profile.png"
              alt="banner-about"
              class="img-fluid img-about"
            />
          </div>
          <div class="col-lg-6 col-md-12 site-title-about">
            <h1 class="font-weight-bold">About</h1>
            <h5 class="pr-lg-5 text-justify">
              Seorang Front End Developer dan juga seorang Junior Network
              Administrator yang terjun ke dunia Programming sejak tahun 2019.
              <p></p>
              Dengan bekal pembelajaran dari bootcamp dan latihan mandiri yang
              saya lakukan, saya bisa membuat aplikasi web maupun mobile dengan
              kemampuan yang saya miliki.
              <p></p>
              Bahasa yang saya gunakan dalam membuat suatu aplikasi Web dan
              Mobile adalah Javascript dengan Framework mereka seperti Vue untuk
              Web dan React Native untuk aplikasi Mobile.
            </h5>
            <div>
              <a
                href="https://drive.google.com/file/d/1hFO2OYV9tRRlaOqTph8eM8dWtgu6RBGx/view?usp=sharing"
                target="_blank"
              >
                <button class="btn-custom color-btn-wa mr-4">
                  Download CV
                </button>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- ================ End ABOUT ================= -->
    <!-- ================ SKILL ================= -->
    <!-- <section class="site-skils">
      <div class="container">
        <div class="row">
          <div class="col-lg-3 col-sm-6 mt-4">
            <div class="feature_item">
              <img src="../assets/img/vue.png" alt="vue" />
              <h4>Web design</h4>
              <p>
                We do many things to make our website look attractive with
                beautiful designs.
              </p>
            </div>
          </div>
          <div class="col-lg-3 col-sm-6 mt-4">
            <div class="feature_item">
              <img src="../assets/img/react.png" alt="vue" />
              <h4>Web design</h4>
              <p>
                We do many things to make our website look attractive with
                beautiful designs.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section> -->
    <!-- ================ End SKILL ================= -->
    <!-- ================ Portofolio ================= -->
    <section id="portofolio" class="site-porto">
      <div class="container">
        <div class="row" style="place-content: center;">
          <div class="col-lg-12 col-md-12">
            <h1 class="font-weight-bold text-center">Portofolio</h1>
          </div>
          <div
            v-for="(data, index) in items"
            :key="index"
            class="col-lg-4 col-md-4 cards"
          >
            <div class="content card-item">
              <div class="content-overlay"></div>
              <div class="card-image">
                <img
                  class="content-image img-fluid"
                  :src="data.image"
                  :alt="data.image"
                />
              </div>
              <div class="content-details fadeIn-left">
                <h5 class="card-title">{{ data.title }}</h5>
                <!-- <p class="card-intro">This is a short description</p> -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- ================ End Portofolio ================= -->
    <!-- ================ Contact ================= -->
    <section id="contact" class="site-contact">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 col-md-12">
            <h1 class="font-weight-bold text-center">Contact</h1>
          </div>
          <div class="col-lg-6 col-md-6 col-sm-12 col-custom br-custom">
            <div class="row">
              <div class="col-md-2 col-sm-12">
                <i
                  class="fa fa-home border-icon p-3"
                  style="font-size: 28px; color: #eea271;"
                ></i>
              </div>
              <div class="col-md-10 mt-2">
                <b style="font-size: 19px;"
                  >Jl. Jakarta Gang Perjuangan No.12 RT72
                </b>
                <br />
                <span style="font-size: 16px;"
                  >Loa Bakung, Sungai Kunjang, Samarinda</span
                >
              </div>
              <br />
              <div class="col-md-2 col-sm-12 mt-3">
                <i
                  class="fa fa-phone border-icon p-3"
                  style="font-size: 28px; color: #eea271;"
                ></i>
              </div>
              <div class="col-md-10 mt-4">
                <b style="font-size: 19px;">+62 831 5344 0780 </b>
                <br />
                <span style="font-size: 16px;">No HP & WhatsApp</span>
              </div>
              <br />
              <div class="col-md-2 col-sm-12 mt-3">
                <i
                  class="fa fa-envelope border-icon p-3"
                  style="font-size: 28px; color: #eea271;"
                ></i>
              </div>
              <div class="col-md-10 mt-4 mb-2">
                <b style="font-size: 19px;">sandy.adzim@gmail.com </b>
                <br />
                <span style="font-size: 16px;">Email Saya</span>
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-md-6 col-sm-12 text-center">
            <div class="row">
              <div class="col-md-12 mt-2">
                <img
                  src="../assets/img/logo-2.png"
                  alt="logo-footer"
                  class="mt-3"
                  style="width: 150px;"
                />
              </div>
              <div class="col-md-12 mt-3">
                <h5>
                  <b style="border-bottom: 2px solid #eea271;" class="pb-1"
                    >Follow Saya</b
                  >
                </h5>
              </div>
              <div class="col-md-12 mt-2">
                <a
                  href="https://www.instagram.com/rahmansyah_sandy/"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <span class="mr-1">
                    <img src="~/assets/img/instagram.png" alt="insta" />
                  </span>
                </a>
                <a
                  href="https://www.facebook.com/adzim.kemuning/"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <span class="mr-1">
                    <img src="~/assets/img/facebook.png" alt="facebook" />
                  </span>
                </a>
                <a
                  href="https://www.linkedin.com/in/sandy-rahmansyah-578322128/"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <span class="mr-1">
                    <img src="~/assets/img/linkedin.png" alt="linkedin" />
                  </span>
                </a>
                <a
                  href="https://github.com/sandyadzim"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  <span class="mr-1">
                    <img src="~/assets/img/github.png" alt="github" />
                  </span>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <div class="custom-footer text-center text-white">
      Copyright @2020 | Sandy Rahmansyah
    </div>
    <!-- ================ End Contact ================= -->
  </div>
</template>

<script>
export default {
  name: 'Portofolio',
  data: () => ({
    items: [
      {
        image: require('../assets/img/pr1.png'),
        title: 'Dashboard Live Test Edutore by Gramedia',
      },
      {
        image: require('../assets/img/pr2.png'),
        title: 'Live Test Edutore by Gramedia',
      },
      {
        image: require('../assets/img/pr7.png'),
        title: 'LMS Academy Edutore by Gramedia (Slicing)',
      },
      {
        image: require('../assets/img/pr3.png'),
        title: 'SKY-ROOM',
      },
      {
        image: require('../assets/img/pr5.png'),
        title: 'JOGJA',
      },
      {
        image: require('../assets/img/pr4.png'),
        title: 'SKY-TOON',
      },
      {
        image: require('../assets/img/pr6.png'),
        title: 'Dashboard SKY-LAN',
      },
      {
        image: require('../assets/img/pr8.png'),
        title: 'Admin Dashboard LMS Academy Edutore by Gramedia',
      },
    ],
  }),
}
</script>

<style scoped>
.content {
  position: relative;
  width: 90%;
  max-width: 400px;
  margin: auto;
  overflow: hidden;
}

.content .content-overlay {
  background: rgba(238, 162, 113, 0.7);
  position: absolute;
  height: 100%;
  width: 100%;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  opacity: 0;
  -webkit-transition: all 0.4s ease-in-out 0s;
  -moz-transition: all 0.4s ease-in-out 0s;
  transition: all 0.4s ease-in-out 0s;
}

.content:hover .content-overlay {
  opacity: 1;
}

.content-image {
  width: 100%;
}

.content-details {
  position: absolute;
  text-align: center;
  padding-left: 1em;
  padding-right: 1em;
  width: 100%;
  top: 50%;
  left: 50%;
  opacity: 0;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  -webkit-transition: all 0.3s ease-in-out 0s;
  -moz-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

.content:hover .content-details {
  top: 50%;
  left: 50%;
  opacity: 1;
}

.content-details h5 {
  color: #fff;
  font-weight: 500;
  letter-spacing: 0.15em;
  margin-bottom: 0.5em;
  text-transform: uppercase;
}

.content-details p {
  color: #fff;
  font-size: 0.8em;
}
.fadeIn-left {
  left: 20%;
}
.cards {
  display: flex;
  padding: 1rem;
  margin-bottom: 2rem;
  width: 100%;
}
@media (min-width: 40rem) {
  .cards {
    width: 50%;
  }
}
@media (min-width: 56rem) {
  .cards {
    width: 33.3%;
  }
}
@media (max-width: 321.98px) {
  .col-custom {
    text-align: center;
  }
}
.card-item:hover {
  cursor: pointer;
  transform: scale(1.1);
  -webkit-transform: scale(1.1);
}
.card-item:hover .card-image {
  opacity: 1;
}
.card-info {
  display: flex;
  flex: 1 1 auto;
  flex-direction: column;
  padding: 1rem;
  line-height: 1.5em;
}
.card-title {
  /* font-size: 25px; */
  line-height: 1.1em;
  color: #32325d;
  margin-bottom: 0.2em;
}
.card-image {
  height: 200px;
  overflow: hidden;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  border-radius: 6px 6px 0px 0px;
  opacity: 0.91;
}
.card-custom {
  border-radius: 8px;
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.4);
}
.site-title {
  padding-top: 18%;
  padding-left: 10%;
}
.site-title-about {
  padding-top: 14%;
  padding-left: 1%;
}
.site-home {
  background: url('../assets/img/bg-pg-1-new-again.png') no-repeat center;
  background-size: cover;
  width: 100%;
}
.site-about {
  background: url('../assets/img/bg-pg-2-new-2.png') no-repeat center;
  background-size: cover;
  width: 100%;
  /* padding-top: 10%; */
}
.site-porto {
  background: url('../assets/img/bg-pg-3-new-again.png') no-repeat center;
  background-size: cover;
  width: 100%;
  padding: 0 0;
}
.site-contact {
  /* background: url('../assets/img/bg-pg-2-new.png') no-repeat center; */
  /* background-size: cover;
  width: 100%; */
  padding: 3rem 0;
}
.banner-image > img {
  padding: 6rem 0;
}
.img-about {
  padding-top: 8rem;
}
.btn-custom {
  width: 150px;
  font-size: 16px;
  font-weight: 600;
  color: #fff;
  cursor: pointer;
  margin: 10px;
  height: 55px;
  text-align: center;
  border: none;
  background-size: 300% 100%;

  border-radius: 50px;
  -moz-transition: all 0.4s ease-in-out;
  -o-transition: all 0.4s ease-in-out;
  -webkit-transition: all 0.4s ease-in-out;
  transition: all 0.4s ease-in-out;
}
.btn-custom:hover {
  background-position: 100% 0;
  -moz-transition: all 0.4s ease-in-out;
  -o-transition: all 0.4s ease-in-out;
  -webkit-transition: all 0.4s ease-in-out;
  transition: all 0.4s ease-in-out;
}
.btn-custom:focus {
  outline: none;
}
.color-btn-wa {
  background-image: linear-gradient(
    to right,
    #fc6076,
    #ff9a44,
    #eea271,
    #e75516
  );
  box-shadow: 0 4px 15px 0 rgba(252, 104, 110, 0.75);
}
.color-btn-email {
  background-image: linear-gradient(
    to right,
    #29323c,
    #485563,
    #2b5876,
    #4e4376
  );
  box-shadow: 0 4px 15px 0 rgba(45, 54, 65, 0.75);
}
.feature_item {
  background: #f7e7dc;
  padding: 45px 25px;
  /* padding: 45px 25px;
  text-align: center;
  background: #f7e7dc;
  cursor: pointer;
  margin-bottom: 30px;
  -webkit-transition: all 0.4s ease 0s;
  -moz-transition: all 0.4s ease 0s;
  -o-transition: all 0.4s ease 0s;
  transition: all 0.4s ease 0s; */
}
.border-icon {
  border: 5px solid #eea271;
  border-radius: 50%;
}
.br-custom {
  border-right: 3px solid #eea271;
}
@media (max-width: 767.98px) {
  .br-custom {
    border-right: 0;
    border-bottom: 3px solid #eea271;
  }
}
.custom-footer {
  padding: 0.75rem 1.25rem;
  background-color: rgb(238, 162, 113);
  border-top: 1px solid rgba(0, 0, 0, 0.125);
}
</style>
