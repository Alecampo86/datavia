<template>
  <section id="background">
    <nuxt-link to="/">
      <div class="icon-menu">
        <!-- <div class="logo"> -->
        <img
          src="~assets/datavia-assets/datavia-assets/icons/icon-home.svg"
          alt=""
        />
        <small>MENU</small>
        <!-- </div> -->
      </div>
    </nuxt-link>

    <div class="box-3">
      <img
        class="box-icon-cam"
        src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
      />
      <h2 class="text-white ml-3">Camera Management</h2>
    </div>

    <div class="container">
      <nuxt-link to="/camera-add">
        <button class="btn cam-btn">
          <img
            class="gear fas fa-cog"
            src="~assets/datavia-assets/datavia-assets/icons/icon-setup.svg"
          />Add New Camera
        </button>
      </nuxt-link>
    </div>
    <button class="btn cancel-btn">Cancel</button>
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

.container {
  width: 91%;
  height: 60%;
  margin: 0 auto;

  background-size: 100%;
  background-position: center center;
  background-size: cover;
  position: absolute;
  top: 23%;
  left: 5%;
  max-width: 1407px;
  display: flex;
  align-items: center;
  justify-content: center;
  border: #3b4e5a solid;
  border-style: dashed;
  border-radius: 20px;
}

.fa-cog:before {
  content: "\f013";
  font-size: 28px;
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

.cam-btn {
  color: #ccc;
  height: 54px;
  width: 200px;
  background: #648498;
  border-radius: 10px;
  transition: all 200ms;
  font-size: 12px;
}

.cam-btn:hover {
  background: #fafafa;
  font-size: 14px;
}

.container h1 {
  font-size: 70px;
  font-family: "Roboto";
  font-weight: 100;
  color: #85b0cb;

  line-height: 80px;
  letter-spacing: 5px;
}

.verathena-box {
  font-size: 82px;
  position: absolute;
  top: 70px;
  left: 66px;
}

.box-2 {
  width: 1235px;
  height: 60px;
  position: absolute;
  top: 358px;
  left: 171px;
  border-top: solid black;
}

.box-3 {
  display: -webkit-box;
  display: flex;
  -webkit-box-align: baseline;
  align-items: baseline;
  width: 292px;
  height: 135px;
  top: 10%;
  left: 44%;
  position: absolute;
}

.box-3 .box-icon-cam {
  width: 20%;
  position: absolute;
  top: -10%;
  left: -18%;
}

.box-3 h3 {
  align-self: end;
  color: #ccc;
  position: absolute;
  left: 75px;
  top: 11px;
  font-size: 16px;
}

.box-4 {
  display: flex;

  align-items: baseline;
  width: 245px;
  height: 135px;
  top: 264px;
  left: 895px;
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
  top: 264px;
  left: 1140px;
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

.btn {
  color: black;
  background: #85b0cb;
  display: -webkit-box;
  display: flex;
  -webkit-box-align: center;
  align-items: center;
  -webkit-box-pack: center;
  justify-content: space-evenly;
  -webkit-transition: all 300ms;
  transition: all 300ms;
  align-content: flex-start;
}

.cancel-btn {
  color: black;
  height: 35px;
  width: 130px;
  background: #85b0cb;
  position: absolute;
  bottom: 8%;
  left: 47%;
  width: 120px;
  border-radius: 10px;
  transition: all 100ms;
  font-size: 12px;
}

.cancel-btn:hover {
  background: #fafafa;
  font-size: 14px;
}

.btn img {
  width: 27px;
}

.btn:hover .fa-cog[data-v-58b8df42] {
  content: "\f013";
  font-size: 35px;
  animation-name: rotate-gear;
  animation-duration: 3s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}

@keyframes rotate-gear {
  from {
    transform: rotateZ(0deg);
  }
  to {
    transform: rotateZ(360deg);
  }
}

/* ///////////////////////Iphone ///////////////////////////////////////////////////// */
@media (min-width: 360px) and (max-width: 469px) {
  .container {
    width: 72%;
    height: 33%;
    top: 30%;
    left: 15%;
  }

  .box-3 {
    top: 20%;
    left: 32%;
    width: 80%;
    height: 8%;
  }

  .icon-menu {
    width: 38px;
    top: 2%;
    left: 4%;
  }

  .cam-btn {
    height: 45px;
    width: 156px;
  }
  .cancel-btn {
    bottom: 25%;
    left: 35%;
  }

  .box-icon-cam {
    width: 20%;
    position: absolute;
    top: -22% !important;
    left: -18%;
}
}

/* /////////////////////////IPAD//////////////////////// */
@media (min-width: 470px) and (max-width: 1250px) {
  .container {
    width: 86%;
    height: 42%;
    top: 15%;
    left: 7%;
  }

  .icon-menu {
    width: 38px;
    top: 3%;
    left: 4%;
  }

  .cam-btn {
    height: 45px;
    width: 156px;
  }

  .box-3 {
    left: 38%;
    top: 9%;
  }

  .box-icon-cam {
    width: 20%;
    position: absolute;
    top: -10%;
    left: 0;
  }

  .cancel-btn {
    bottom: 35%;
    left: 43%;
  }
}
</style>
