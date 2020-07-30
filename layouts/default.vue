<template>
  <div>
    <b-navbar toggleable="lg" type="light" class="nav-custom" sticky>
      <div class="container">
        <b-navbar-brand href="#">
          <img
            src="../assets/img/logo-2.png"
            alt="logo"
            style="width: 150px; height: auto;"
          />
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-navbar-nav>
              <li class="nav-item px-2" style="font-size: 20px;">
                <a href="#home" target="_self" class="nav-link text-nav"
                  >Home</a
                >
              </li>
              <li class="nav-item px-2" style="font-size: 20px;">
                <a href="#about" target="_self" class="nav-link text-nav"
                  >About</a
                >
              </li>
              <li class="nav-item px-2" style="font-size: 20px;">
                <a href="#portofolio" target="_self" class="nav-link text-nav"
                  >Portofolio</a
                >
              </li>
              <li class="nav-item px-2" style="font-size: 20px;">
                <a href="#contact" target="_self" class="nav-link text-nav"
                  >Contact</a
                >
              </li>
            </b-navbar-nav>
          </b-navbar-nav>
        </b-collapse>
      </div>
    </b-navbar>
    <Nuxt />
  </div>
</template>

<style>
html {
  /* font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box; */
  scroll-behavior: smooth;
}

/* *,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
} */
.nav-custom {
  background-color: #fff;
  border-bottom: 1px solid rgb(187, 187, 187);
  box-shadow: 0 4px 4px rgba(0, 0, 0, 0.2);
}
.text-nav {
  color: #eea271 !important;
  font-size: 28 !important;
}
@font-face {
  font-family: ElliotSans-Medium;
  font-style: normal;
  font-weight: 400;
  src: local('ElliotSans-Medium'),
    url(../assets/font/ElliotSans-Medium.woff) format('woff');
}
@font-face {
  font-family: 'Elliot Sans Medium Italic';
  font-style: normal;
  font-weight: 400;
  src: local('Elliot Sans Medium Italic'),
    url(../assets/font/ElliotSans-MediumItalic.woff) format('woff');
}
@font-face {
  font-family: ElliotSans-Regular;
  font-style: normal;
  font-weight: 400;
  src: local('ElliotSans-Regular'),
    url(../assets/font/ElliotSans-Regular.woff) format('woff');
}
@font-face {
  font-family: 'Elliot Sans Italic';
  font-style: normal;
  font-weight: 400;
  src: local('Elliot Sans Italic'),
    url(../assets/font/ElliotSans-RegularItalic.woff) format('woff');
}
@font-face {
  font-family: ElliotSans-Light;
  font-style: normal;
  font-weight: 400;
  src: local('ElliotSans-Light'),
    url(../assets/font/ElliotSans-Light.woff) format('woff');
}
@font-face {
  font-family: 'Elliot Sans Light Italic';
  font-style: normal;
  font-weight: 400;
  src: local('Elliot Sans Light Italic'),
    url(../assets/font/ElliotSans-LightItalic.woff) format('woff');
}
@font-face {
  font-family: ElliotSans-Bold;
  font-style: normal;
  font-weight: 400;
  src: local('ElliotSans-Bold'),
    url(../assets/font/ElliotSans-Bold.woff) format('woff');
}
@font-face {
  font-family: 'Elliot Sans Bold Italic';
  font-style: normal;
  font-weight: 400;
  src: local('Elliot Sans Bold Italic'),
    url(../assets/font/ElliotSans-BoldItalic.woff) format('woff');
}
body {
  font-family: ElliotSans-Regular;
  font-size: 14px;
  font-weight: 400;
}
</style>
