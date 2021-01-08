<template>
  <div class="wrap">
    <img
      class="wrap-img"
      src="~assets/datavia-assets/datavia-assets/images/datavia-background.jpg"
      alt=""
    />
    <div class="logo">
      <img
        src="~assets/datavia-assets/datavia-assets/logo/datavia_logo_w.svg"
        alt=""
      />
    </div>
    <div class="verathena-box">
      <h1>WELCOME TO VERATHENA<small>&#8482;</small> PLATFORM</h1>
    </div>

    <div class="box-2"></div>
    <!-- ////////////////////////////////ICON CAM/////////////////////////////////////// -->
    <div class="box-group">
      <nuxt-link to="/camera-management">
        <div class="box-3">
          <img
            class="box-icon-cam"
            src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
          />
          <!-- <h3>Camera Management</h3> -->

          <div class="arrow-hover">
            <h3>Camera Management</h3>
            <img
              class="box-arrow"
              src="~assets/datavia-assets/datavia-assets/icons/icon-arrow.svg"
            />
          </div>
        </div>
      </nuxt-link>
      <!-- ////////////////////////////////ICON AI/////////////////////////////////////// -->
      <div class="box-4">
        <img
          class="box-icon-ai"
          src="~assets/datavia-assets/datavia-assets/icons/icon-ai-sensing.svg"
        />
        <!-- <h3>Configuration Management</h3> -->
        <div class="arrow-hover2">
          <div class="menu-bar">
            <h3>Configuration Management</h3>
          </div>
          <img
            class="box4-arrow"
            src="~assets/datavia-assets/datavia-assets/icons/icon-arrow.svg"
          />
        </div>
      </div>
      <!-- ////////////////////////////////ICON DASH/////////////////////////////////////// -->
      <div class="box-5">
        <img
          class="box-icon-dash"
          src="~assets/datavia-assets/datavia-assets/icons/icon-dashboard-report.svg"
        />
        <!-- <h3>Intelligent Dashboard</h3> -->
        <div class="arrow-hover3">
          <div class="menu-bar2">
            <h3>Intelligent Dashboard</h3>
          </div>
          <img
            class="box5-arrow"
            src="~assets/datavia-assets/datavia-assets/icons/icon-arrow.svg"
          />
        </div>
      </div>
    </div>
  </div>
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

.box-group {
  width: 55%;
  height: 50%;
  position: absolute;
  border: 0;
  bottom: 0;
  right: 0%;
}

.wrap {
  height: 100%;
  margin: 0 auto;
  margin-top: 80px;
  position: relative;
  width: 90%;
}

#background {
  background: #191a1d;
  height: 48em;
}

.logo {
  width: 18%;
  margin: 0%;
  margin-left: 0%;
  cursor: pointer;
  position: absolute;
  top: 5%;
  margin-left: 3%;
}

.wrap h1 {
  font-size: 70px;
  font-family: "Roboto";
  font-weight: 100;
  color: #85b0cb;

  line-height: 80px;
  letter-spacing: 5px;
}

.wrap-img {
  width: 100%;
}

.verathena-box {
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
  flex-flow: row wrap;
  width: 44%;
  top: 37%;
  position: absolute;
  left: 8%;
}

.box-2 {
  width: 92%;

  position: absolute;
  top: 76%;
  left: 8%;
  border-top: solid black;
}

.box-3 {
  display: -webkit-box;
  display: flex;
  -webkit-box-align: baseline;
  align-items: baseline;
  width: 245px;
  height: 135px;
  top: 21%;
  left: 0;
  position: absolute;
}

.menu-bar {
  display: -webkit-box;
  display: flex;
  width: 6%;

  position: absolute;
  top: 15%;
}

.box-3 .box-icon-cam {
  width: 45%;
}

.box-3 h3 {
  align-self: flex-end;
  color: #85b0cb;
  position: absolute;
  left: 0px;
  font-size: 14px;
}

.box-4 {
  display: -webkit-box;
    display: flex;
    -webkit-box-align: baseline;
    align-items: baseline;
    width: 59%;
    position: absolute;
    top: 0%;
    left: 26%;
}

.box-4 .box-icon-ai {
  width: 45%;
}

.menu-bar{
    display: -webkit-box;
    display: flex;
    width: 194%;
    position: absolute;
    top: 165%;
    left: -32%;
}

.menu-bar2{
    display: -webkit-box;
    display: flex;
    width: 194%;
    position: absolute;
    top: 165%;
    left: -32%;
}

.box-4 h3 {
  align-self: flex-end;
  color: #85b0cb;
  position: absolute;
  left: 0px;
  font-size: 14px;
}

.box-5 {
    display: -webkit-box;
    display: flex;
    -webkit-box-align: baseline;
    align-items: baseline;
    width: 59%;
    position: absolute;
    top: 80%;
    left: 35%;
}

.box-5 .box-icon-dash {
  width: 45%;
}

.box-5 h3 {
  align-self: flex-end;
  color: #85b0cb;
  position: absolute;
  left: 0px;
  font-size: 14px;
}

.arrow-hover {
  position: absolute;
  top: 94px;
  width: 97%;
  height: 43px;
  cursor: pointer;
  transition: all 300ms;
}

.arrow-hover h3 {
  position: absolute;
  top: 10%;
  font-family: roboto;
}

.arrow-hover2 {
  position: absolute;
    top: 60%;
    width: 70%;
    height: 0;
    cursor: pointer;
    -webkit-transition: all 300ms;
    transition: all 300ms;

    left: 6%;
}

.arrow-hover2 h3 {
  position: absolute;
  top: 45%;
  font-family: roboto;
}

.arrow-hover3 {
  position: absolute;
  top: 94px;
  width: 108%;
  height: 43px;
  cursor: pointer;
  transition: all 300ms;
}

.arrow-hover3 h3 {
  position: absolute;
  top: 45%;
  font-family: roboto;
}

.arrow-hover img {
  width: 5%;
  transform: rotate(270deg);
  position: absolute;
  top: 25%;
  right: 38%;
  transition: all 300ms;
}
.arrow-hover:hover {
  border-top: solid #85b0cb;
  border-width: thick 0 0;
}

.arrow-hover:hover h3 {
  color: white;
}

.arrow-hover2:hover h3 {
  color: white;
}

.arrow-hover3:hover h3 {
  color: white;
}

.arrow-hover:hover img {
  right: 1%;
}

.arrow-hover2:hover {
  border-top: solid #85b0cb;
  border-width: thick 0 0;
}

.arrow-hover2 img {
  width: 5%;
  transform: rotate(270deg);
  position: absolute;
  top: 28%;
  right: 60%;
  transition: all 300ms;
}

.arrow-hover2:hover img {
  right: 1%;
}

.arrow-hover3:hover {
  border-top: solid #85b0cb;
  border-width: thick 0 0;
}

.arrow-hover3 img {
  width: 5%;
  transform: rotate(270deg);
  position: absolute;
  top: 28%;
  right: 63%;
  transition: all 300ms;
}

.arrow-hover3:hover img {
  right: 1%;
}

@media (min-width: 0px) and (max-width: 269px) {
}

/* ///////////////////////Iphone ///////////////////////////////////////////////////// */
@media (min-width: 360px) and (max-width: 469px) {
  .wrap {
    height: 667px;
    margin: 0 auto;

    position: relative;
    width: 100%;
    display: flex;
    align-items: center;
  }

  .wrap-img {
    display: none;
  }

  .logo {
    width: 50%;
    margin: 10px;
    cursor: pointer;
    position: absolute;
    top: 2%;
    left: 23%;
  }

  .wrap h1  {
    font-size: 32px;
    font-family: "Roboto";
    font-weight: 100;
    color: #85b0cb;
    line-height: 52px;
    letter-spacing: 8px;
    position: absolute;
    left: 3%;
}
  .verathena-box {
    font-size: 82px;
    position: absolute;
    top: 15%;
    left: 9%;
    display: -webkit-box;
    display: flex;
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
    flex-flow: row wrap;
    min-width: 82%;
    text-align: center;
  }

  .box-group {
    width: 92%;
    height: 24%;
    position: absolute;
    border: 0;
    bottom: 0;
    right: 0%;
    top: 63%;
    left: 4%;
  }

  .box-2 {
    display: none;
  }

  .box-3 {
    display: -webkit-box;
    display: flex;
    -webkit-box-align: baseline;
    align-items: baseline;
    width: 59%;
    position: absolute;
    top: -80%;
    left: 26%;
}

  .box-icon-cam {
    position: absolute;
    left: 17%;
  }

  .box-icon-dash{
    width: 30%;
    right: 48%;
    position: absolute;
}

  .box-icon-ai{
    position: absolute;
    left: 33%;
    top: 3%;
  }
  .box-3 h3 {
    top: 0;
  }

  .arrow-hover {
    position: absolute;
    top: 60%;
    width: 70%;
    height: 0;
    cursor: pointer;
    -webkit-transition: all 300ms;
    transition: all 300ms;

    left: 6%;
}

  .arrow-hover h3{
    position: absolute;
    top: 10%;
    font-family: roboto;
    font-size: 14px;
    font-weight: 100;
    color: white;
}

  .arrow-hover img{
    display: none;
  }

  .arrow-hover2 img{
    display: none;
  }

  .arrow-hover2 h3{
    position: absolute;
    top: 10%;
    font-family: roboto;
    font-size: 14px;
    font-weight: 100;
    color: white;
}

  .arrow-hover3 img{
    display: none;
  }

  .arrow-hover3 h3{
    position: absolute;
    top: 10%;
    font-family: roboto;
    font-size: 14px;
    font-weight: 100;
    color: white;
}

  .arrow-hover:hover{
    display: none;
  }

  .arrow-hover2:hover{
    display: none;
  }

  .arrow-hover3:hover{
    display: none;
  }



  .arrow-hover2 {
    position: absolute;
    top: 26%;
    width: 70%;
    height: 43px;
    cursor: pointer;
    -webkit-transition: all 300ms;
    transition: all 300ms;
    text-align: center;
    left: 15%;
}

  .arrow-hover3 {
    position: absolute;
    top: 30%;
    width: 97%;
    height: 43px;
    cursor: pointer;
    -webkit-transition: all 300ms;
    transition: all 300ms;
    text-align: center;
    right: -15%;
    top: 28%;
}

.box5-arrow{
  display: none;
}

  .box-4 {
    display: flex;
    -webkit-box-align: baseline;
    align-items: baseline;
    width: 42%;
    position: absolute;
  }

  .box-4 h3 {
    top: 0;
  }

  .box-5 {
    display: -webkit-box;
    display: flex;
    -webkit-box-align: baseline;
    align-items: baseline;
    width: 50%;
    position: absolute;
}

  .box-5 h3 {
    top: 0;
  }
}

/* /////////////////////////IPAD//////////////////////// */
@media (min-width: 470px) and (max-width: 1250px) {
  .wrap {
    height: 1024px;
    margin: 0 auto;
    position: relative;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }



  .wrap-img {
    width: 400%;
  }

  .logo {
    width: 30%;
    margin: 10px;
    cursor: pointer;
    position: absolute;
    top: 4%;
    left: 34%;
  }

  .wrap h1 {
    font-size: 50px;
    font-family: "Roboto";
    font-weight: 100;
    color: #85b0cb;
    line-height: 52px;
    letter-spacing: 5px;
  }

  .verathena-box {
    font-size: 82px;
    position: absolute;
    top: 19%;
    left: 9%;
    display: -webkit-box;
    display: flex;
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
    flex-flow: row wrap;
    min-width: 82%;
    text-align: center;
  }

  .wrap h1 {
    font-size: 44px;
    font-family: "Roboto";
    font-weight: 300;
    color: #85b0cb;
    line-height: 52px;
    letter-spacing: 5px;
  }

  .box-group {
    width: 92%;
    height: 24%;
    position: absolute;
    border: 0;
    bottom: 0;
    right: 0%;
    top: 35%;
    left: 6%;
  }

  .box-3 {
    display: -webkit-box;
    display: flex;
    -webkit-box-align: baseline;
    align-items: baseline;
    width: 30%;
    margin: 10%;
    position: absolute;
  }
  .box-3 h3 {
    top: 0;
  }

  .arrow-hover {
    position: absolute;
    top: 52%;
    width: 97%;
    height: 43px;
    cursor: pointer;
    -webkit-transition: all 300ms;
    transition: all 300ms;
    left: -29%;
    text-align: center;
  }

  .arrow-hover h3 {
    position: absolute;
    top: 10%;
    font-family: roboto;
    left: 19%;
  }

  .arrow-hover2 {
    position: absolute;
    top: 52%;
    width: 97%;
    height: 43px;
    cursor: pointer;
    -webkit-transition: all 300ms;
    transition: all 300ms;
    left: -33%;
    text-align: center;
  }

  .arrow-hover2 h3 {
    position: absolute;
    top: 10%;
    font-family: roboto;
    left: 459%;
  }

  .arrow-hover3 {
    position: absolute;
    top: 52%;
    width: 97%;
    height: 43px;
    cursor: pointer;
    -webkit-transition: all 300ms;
    transition: all 300ms;
    left: -33%;
    text-align: center;
  }
  .arrow-hover3 h3 {
    position: absolute;
    top: 10%;
    font-family: roboto;
    left: 588%;
    top: -3px;
  }

  .arrow-hover:hover {
    border-top: solid #85b0cb;
    border-width: thick 0 0;
  }

  .arrow-hover2:hover {
    border-top: solid #85b0cb;
    border-width: thick 0 0;
  }

  .arrow-hover3:hover {
    border-top: solid #85b0cb;
    border-width: thick 0 0;
  }
  .arrow-hover img {
    display: none;
  }

  .arrow-hover2 img {
    display: none;
  }

  .arrow-hover3 img {
    display: none;
  }

  .box-4 {
    display: -webkit-box;
    display: flex;
    -webkit-box-align: baseline;
    align-items: baseline;
    width: 30%;
    position: absolute;
    margin: 10%;
  }

  .box-4 h3 {
    top: 0;
  }

  .box-5 {
    display: -webkit-box;
    display: flex;
    -webkit-box-align: baseline;
    align-items: baseline;
    width: 30%;
    position: absolute;
    margin: 10%;
  }

  .box-5 h3 {
    top: 0;
  }
}
</style>
