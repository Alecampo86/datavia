<template>
  <div class="container">
    <img
      class="container-img"
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
      <h1>WELCOME TO VERATHENA <small>&#8482;</small> PLATFORM</h1>
    </div>

    <div class="box-2"></div>
    <!-- ////////////////////////////////ICON CAM/////////////////////////////////////// -->
    <nuxt-link to="/camera-management">
      <div class="box-3">
        <img
          class="box-icon-cam"
          src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
        />
        <h3>Camera Management</h3>

        <div class="arrow-hover">
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
      <h3>Configuration Management</h3>
      <div class="arrow-hover2">
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
      <h3>Intelligent Dashboard</h3>
      <div class="arrow-hover3">
        <img
          class="box5-arrow"
          src="~assets/datavia-assets/datavia-assets/icons/icon-arrow.svg"
        />
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

/* .container {

  margin: 0 auto;
  background-position: center center;
  background-size: cover;
  position: absolute;
  top: 30px;
  left: 55px;
  max-width: 1407px;
} */

.container {
  height: 100vh;
  max-width: 1407px;
  margin: 0 auto;
  margin-top: 80px;
}

#background {
  background: #191a1d;
  height: 48em;
}

.logo {
  width: 200px;
  margin: 10px;
  cursor: pointer;
  position: absolute;
  top: 74px;
}

.container h1 {
  font-size: 70px;
  font-family: "Roboto";
  font-weight: 100;
  color: #85b0cb;

  line-height: 80px;
  letter-spacing: 5px;
}

.container-img {
  width: 100%;
}

.verathena-box {
  font-size: 82px;
  position: absolute;
  top: 214px;
  left: 113px;

  display: flex;
  flex-flow: row wrap;
  width: 522px;
}

.box-2 {
  width: 1340px;
  height: 60px;
  position: absolute;
  top: 458px;
  left: 120px;
  border-top: solid black;
}

.box-3 {
  display: flex;

  align-items: baseline;
  width: 245px;
  height: 135px;
  top: 364px;
  left: 650px;
  position: absolute;
}

.box-3 .box-icon-cam {
  width: 35%;
}

.box-3 h3 {
  align-self: flex-end;
  color: #85b0cb;
  position: absolute;
  left: 0px;
  font-size: 14px;
}

.box-4 {
  display: flex;

  align-items: baseline;
  width: 245px;
  height: 135px;
  top: 364px;
  left: 920px;
  position: absolute;
}

.box-4 .box-icon-ai {
  width: 23%;
}

.box-4 h3 {
  align-self: flex-end;
  color: #85b0cb;
  position: absolute;
  left: 0px;
  font-size: 14px;
}

.box-5 {
  display: flex;

  align-items: baseline;
  width: 245px;
  height: 135px;
  top: 364px;
  left: 1198px;
  position: absolute;
}

.box-5 .box-icon-dash {
  width: 30%;
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
  width: 245px;
  height: 43px;
  cursor: pointer;
  transition: all 100ms;
}

.arrow-hover2 {
  position: absolute;
  top: 94px;
  width: 245px;
  height: 43px;
  cursor: pointer;
  transition: all 100ms;
}

.arrow-hover3 {
  position: absolute;
  top: 94px;
  width: 245px;
  height: 43px;
  cursor: pointer;
  transition: all 300ms;
}

.arrow-hover img {
  width: 5%;
  transform: rotate(270deg);
  position: absolute;
  top: 25px;
  right: 85px;
  transition: all 300ms;
}
.arrow-hover:hover {
  border-top: solid #85b0cb;
  color: aliceblue;
}

.arrow-hover:hover img {
  right: 5px;
}

.arrow-hover2:hover {
  border-top: solid #85b0cb;
}

.arrow-hover2 img {
  width: 5%;
  transform: rotate(270deg);
  position: absolute;
  top: 25px;
  right: 47px;
  transition: all 300ms;
}

.arrow-hover2:hover img {
  right: 5px;
}

.arrow-hover3:hover {
  border-top: solid #85b0cb;
}

.arrow-hover3 img {
  width: 5%;
  transform: rotate(270deg);
  position: absolute;
  top: 25px;
  right: 85px;
  transition: all 100ms;
}

.arrow-hover3:hover img {
  right: 5px;
}


</style>
