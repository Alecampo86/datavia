<template>
  <section id="background">
    <nuxt-link to="/">
      <div class="icon-menu">
        <img
          src="~assets/datavia-assets/datavia-assets/icons/icon-home.svg"
          alt=""
        />
        <small>MENU</small>
      </div>
    </nuxt-link>

    <div class="box-3">
      <img
        class="box-icon-cam"
        src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
      />
      <h2 class="text-white ml-2">Camera Management</h2>
    </div>

    <!-- ////////////////////////icono home///////////////// -->
    <div class="container row">
      <!-- COLUMNA 1 -->
      <div class="columna1 col col-lg-12 border w-100">
        <div class="cam-corner">
          <img src="~assets/datavia-assets/datavia-assets/images/camera.png" />
        </div>
        <div class="cam-text">
          <small class="cam-span">Camera A1 - Building R1 - Floor 1A</small>
          <small class="text-white">Sony - ABC100</small>
          <img
            src="~assets/datavia-assets/datavia-assets/icons/Icon-battery-quarter.svg"
            alt=""
          />
        </div>

        <hr class="line" />

        <div class="temp-calib">
          <div class="temp-box"><span class="number">2</span></div>
          <div class="temp-box1"><span class="number">1</span></div>
          <div class="temp-box1"><span class="number">0</span></div>
          <div class="temp-box1"><span class="number">-1</span></div>
          <div class="temp-box"><span class="number">-2</span></div>
        </div>

        <div class="col-lg-6 calib-pic w-100 mt-5">
          <img src="~assets/images/public-recog.jpg" />
        </div>

        <div class="calib-box h-75">
          <div class="calib-lines">
            <hr class="calib-lineA" />
            <hr class="calib-lineB" />
            <hr class="calib-lineC" />
          </div>
          <div class="calib-box-textA">
            <span class="text-white">0</span>
            <span class="text-white">0.3</span>
            <span class="text-white">3</span>
            <span class="text-white">5</span>
            <span class="text-white">10</span>
            <span class="text-white">15</span>
          </div>
          <div class="calib-box-textB">
            <span class="text-white">250</span>
            <span class="text-white">F11</span>
            <span class="text-white">200</span>
          </div>
          <span class="calib-length">L</span>
          <img
            class="calib-iso"
            src="~assets/datavia-assets/datavia-assets/icons/icon-iso.svg"
          />
          <div class="calib-box-textC">
            <div>
              <small class="text-white text-align-center">Zoom Level</small>
            </div>
            <small class="text-white">Brightness Level</small>
            <small class="text-white">Contrast Level</small>
          </div>

          <div>
            <button class="btn calib-cancel">
              <i class="far fa-window-close"></i>
              Cancel
            </button>
          </div>

          <div class="save-continue">
            <nuxt-link to="/camera-save">
              <button class="btn calib-save">
                <img
                  class="icon-save"
                  src="~assets/datavia-assets/datavia-assets/icons/icon-save.svg"
                />Save and Continue
              </button>
            </nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
* {
  /* background: #191a1d; */
  /* height: 100vh; */
  margin: 0px;
  padding: 0px;
}

a {
  width: 100%;
  text-align: -webkit-center;
}

.calib-cancel {
  color: black;
  height: 35px;
  width: 130px;
  background: #85b0cb;
  position: absolute;
  bottom: -10px;
  left: 170px;
  width: 120px;
  border-radius: 5px;
  -webkit-transition: all 100ms;
  transition: all 100ms;
  font-size: 12px;
}

.calib-cancel i {
  font-size: 15px;
  position: absolute;
  left: 10px;
  top: 10px;
}
.icon-save {
  position: absolute;
  left: 4px;
  top: 10px;
}
.calib-lines {
  position: absolute;
  top: 20px;
  width: 100%;
  height: 89%;
  display: flex;
  justify-content: center;
  align-items: center;
}
.calib-iso {
  position: absolute;
  bottom: 146px;
  right: 0px;
  width: 32px;
}

.calib-save {
  color: black;
  height: 35px;

  background: #85b0cb;
  position: absolute;
  bottom: -10px;
  left: 312px;
  width: 170px;
  border-radius: 5px;
  -webkit-transition: all 100ms;
  transition: all 100ms;
  font-size: 12px;
}

.flat-btn {
  color: black;
  height: 35px;
  width: 130px;
  background: #85b0cb;
  position: absolute;
  bottom: 200px;
  left: 240px;
  width: 120px;
  border-radius: 5px;
  -webkit-transition: all 100ms;
  transition: all 100ms;
  font-size: 12px;
}

.calib-pic img {
  -o-object-fit: cover;
  object-fit: initial;
  width: 100%;
}

.calib-box {
  position: absolute;
  top: 98px;
  right: 6px;
  width: 513px;
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}

.calib-lineA {
  height: 30px;
  color: #06a0ff;
  width: 40%;
}

.calib-lineB {
  height: 20px;
  color: #aaaaaa;
  width: 20%;
}

.calib-lineC {
  height: 30px;
  color: #06a0ff;
  width: 40%;
}

.calib-box-textA {
  height: 20px;
  width: 99%;
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

.calib-box-textB {
  height: 35px;
  width: 99%;
  position: absolute;
  top: 197px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.calib-length {
  color: #85b0cb;
  font-weight: 900;
  position: absolute;
  font-size: 23px;
  left: 1px;
  bottom: 143px;
}

.calib-box-textC {
  height: 45px;
  width: 99%;
  position: absolute;
  bottom: 100px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.caib-iso {
  position: absolute;
  bottom: 148px;
  right: 1px;
  width: 32px;
}

.container {
  width: 80%;
  height: 630px;
  margin: 0 auto;
  background-size: 100%;
  background-position: center center;
  background-size: cover;
  position: absolute;
  top: 140px;
  left: 142px;
  max-width: 1407px;
  display: -webkit-box;
  display: flex;
  -webkit-box-align: center;
  align-items: center;
  -webkit-box-pack: center;
  justify-content: center;
}

.cam-name {
  position: absolute;
  top: 204px;
}

.form-control {
  border-color: rgb(100, 100, 100);
  cursor: pointer;
}
.cam-description {
  position: absolute;
  bottom: 140px;
  left: 73px;
  width: 454px;
  height: 101px;
}
.cam-name {
  position: absolute;
  top: 204px;
}

.cam-corner {
  position: absolute;
  top: -0px;
  left: 0px;
}

.cam-corner img {
  width: 100px;
}

.form-control:focus {
  border-color: #85b0cb;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 8px #85b0cb;
}

#background {
  background: #191a1d;
  height: 48em;
}

.icon-menu {
  padding: 0;
  cursor: pointer;
  background: #85b0cb;
  border-radius: 7px;
  position: absolute;
  width: 37px;
  -webkit-transition: all 200ms;
  transition: all 200ms;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 38px;
  top: 6%;
  left: 3%;
}

.column-title {
  display: flex;
  /* align-items: center; */
  justify-content: center;
  align-content: center;
}

.column-title img {
  width: 28px;
  position: absolute;
  left: 82px;
  top: 4px;
}

.column-title i {
  content: "\f3c5";
  color: #85b0cb;
  position: absolute;
  left: 80px;
  top: 2px;
  font-size: x-large;
}

.file {
  content: "\f3c5";
  color: #85b0cb;
  position: absolute;
  left: 160px;
  top: 2px;
  font-size: x-large;
}

.icon-menu small {
  display: none;
  color: #fafafa;
  position: absolute;
  top: 12px;
  left: 60px;
}

.icon-menu:hover {
  background: #fafafa;
}

.icon-menu:hover .logo {
  background: #fafafa;
}

.icon-menu:hover small {
  display: block;
}

.logo {
  width: 28px;
  height: 26px;
  margin: 10px;
  cursor: pointer;
  background: #85b0cb;
  position: static;
  transition: all 200ms;
}

.box-3 {
  display: flex;

  align-items: center;
  width: 300px;
  height: 90px;
  top: 35px;
  left: 606px;
  position: absolute;
}

.box-3 .box-icon-cam {
  width: 20%;
}

.box-3 h3 {
  align-self: end;
  color: #ccc;
  position: absolute;
  left: 75px;
  top: 11px;
  font-size: 16px;
}

.columna1 {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  flex-flow: column wrap;
  height: 80%;
  position: absolute;
  top: 3%;

  left: 0%;
}

.columna2 {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  flex-flow: column wrap;
}

.rowSelect {
  display: inline-flex;
  justify-content: space-around;
}
.select1 {
  position: absolute;
  top: 260px;
  left: 74px;
}
.select2 {
  position: absolute;
  top: 316px;
  left: 73px;
}

.columnaBox {
  display: flex;
  align-items: center;
  justify-content: center;
  align-self: initial;
  position: absolute;
  top: 0px;
  cursor: pointer;
}

.flat-btn span {
  position: absolute;
  top: 7px;
  right: 18px;
}

.columnaBox2 {
  position: absolute;
  top: 336px;
}

.icon-success {
  color: greenyellow;
  font-size: 25px;
  position: absolute;
  right: 90px;
  top: 54px;
}

.line {
  color: #dddddd;
  height: 1px;
  position: absolute;
  top: 70px;
  width: 97%;
}

.temp-calib {
  position: absolute;
  top: 99px;
  left: 20px;
  width: 20px;
  height: 75%;
  display: flex;
  flex-flow: column wrap;
  justify-content: space-between;
  border-left: solid white;
  border-top: solid white;
  border-bottom: solid white;
}

.temp-box {
  width: 19px;
}

.temp-box1 {
  border-bottom: solid white;
}

.calib-pic {
  display: -webkit-box;
  display: flex;
  -webkit-box-align: center;

  -webkit-box-pack: center;

  align-self: initial;
  position: absolute;
  top: 50px;
  height: 380px;
  border: solid #85b0cb;

  border-radius: 10px;
  cursor: pointer;
  -o-object-fit: cover;
  object-fit: cover;
  left: 65px;
}

.cam-span {
  color: #85b0cb;
  display: block;
}

.cam-text {
  height: 46px;
  top: 26px;
  position: absolute;
  left: 104px;
  width: 91%;
}

.cam-text img {
  position: absolute;
  right: 25px;
  top: 0px;
}

.number {
  position: absolute;
  color: white;
  left: 24px;
}

.fa-map-marker-alt:before {
  content: "\f3c5";
  position: absolute;
  left: -70px;
}

/* /////////////////////////////////IPHONE/////////////////////////////////////////////////////////// */
@media (min-width: 360px) and (max-width: 469px) {
  #background {
    background: #191a1d;
    height: 48em;
    position: relative;
  }

  .container {
    height: 67%;
    margin: 0 auto;
    background-size: 100%;

    position: absolute;
    top: 16%;
    left: 10%;
    width: 79%;
    display: -webkit-box;

    -webkit-box-align: center;
    align-items: center;
    -webkit-box-pack: center;
  }

  .box-3 {
    top: 8%;
    left: 28%;
    width: 49%;
    height: 8%;
  }

  .box-3 img {
    display: none;
  }

  .icon-menu {
    width: 38px;
    top: 2%;
    left: 4%;
  }

  .rowSelect {
    height: 12%;
    width: 100% !important;
    position: absolute;
    top: 49%;
  }

  .select1 {
    position: absolute;
    top: -2%;
    left: 4%;
    min-width: 41%;
  }

  .select2 {
    position: absolute;
    top: -2%;
    left: 55%;
    min-width: 40%;
  }

  .columnaBox {
    width: 91% !important;
    top: -3%;
  }

  .cam-input {
    width: 120% !important;
    position: absolute;
    top: -7%;
    left: 5%;
  }

  .column-title i {
    width: 10%;
    position: absolute;
    left: 4%;
    top: 1%;
  }

  .columna1 {
    border: none !important;
  }

  .cam-description {
    position: absolute;
    bottom: 10%;
    left: 5%;
    width: 90%;
    height: 24%;
  }

  .columna2 {
    min-width: 102%;
  }

  .url-input {
    width: 100% !important;
    position: absolute;
    top: 7%;
    left: 5%;
  }

  .url {
    width: 90% !important;
  }

  .icon-success {
    right: 14%;
    top: 41%;
  }

  .columnaBox3 {
    width: 96% !important;
    position: absolute;
    top: 3%;
    height: 48%;
  }

  .cam-spectrum {
    position: absolute;
    top: 21%;
    left: 1%;
  }

  .flat-btn {
    position: absolute;
    bottom: 45%;
    left: 27%;
    width: 46%;
  }

  .column-title {
    min-width: 90%;
  }

  .cam-btn {
    height: 45px;
    width: 156px;
  }
  .cancel-btn {
    bottom: 14%;
    left: 30%;
  }

  .save-continue {
    position: absolute;
    bottom: 6px;
    left: -243px;
  }

  .save-btn {
    position: absolute;
    top: 0%;
    left: 0%;
  }

  .calib-box {
    top: 45%;

    width: 100%;
    left: 0;
  }

  .calib-lines {
    width: 115%;
  }

  .calib-cancel {
    position: absolute;
    bottom: -19%;
    left: 34%;
  }

  .calib-pic {
    position: absolute;
    top: 10%;
    height: 45%;
    left: 8%;
  }

  .temp-calib {
    position: absolute;
    top: 22%;
    left: -7%;
    width: 7%;
    height: 43%;
  }

  .calib-box-textB {
    height: 12%;
    width: 120%;
    position: absolute;

    display: -webkit-box;
    display: flex;
    -webkit-box-align: center;
    align-items: center;
    justify-content: space-around;
    top: 56%;
    left: -11%;
  }

  .calib-box-textC {
    bottom: 18%;
    width: 110%;
    left: -5%;
    text-align: center;
  }

  .cam-corner {
    position: absolute;
    top: 0%;
    left: -10%;
  }

  .cam-text {
    height: 46px;
    top: 8px;
    position: absolute;
    left: 29%;
    width: 71%;
  }

  .cam-text img {
    position: absolute;
    right: 16%;
    top: 63%;
  }

  .line {
    display: none;
  }
}
</style>
