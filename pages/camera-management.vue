<template>
  <section id="background">

    <div class="box-3 ">
        <img
          class="box-icon-cam"
          src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
        />
        <h3>Camera Management</h3>

      </div>

    <div class="container">
     <nuxt-link to="/">
       <div class="icon-menu">
          <div class="logo">
            <img
              src="~assets/datavia-assets/datavia-assets/icons/icon-home.svg"
              alt=""
            />
          </div>
       </div>
     </nuxt-link >

      <button class="btn cam-btn">Add New Camera</button>
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

.container {
  width: 96%;
  height: 430px;
  margin: 0 auto;

  background-size: 100%;
  background-position: center center;
  background-size: cover;
  position: absolute;
  top: 116px;
  left: 55px;
  max-width: 1407px;
  display: flex;
  align-items: center;
  justify-content: center;
  border: #3b4e5a solid;
  border-style: dashed;
  border-radius: 20px;
}

#background {
  background: #191a1d;
  height: 48em;
}

.icon-menu{
    padding: 0;
    cursor: pointer;
    background: #648498;
    border-radius: 12px;
    position: absolute;
    top: -86px;
    left: 0px;
    /* display: flex; */
    /* align-items: center; */
}

.logo {
    width: 28px;
    height: 26px;
    margin: 10px;
    cursor: pointer;
    background: #648498;
    position: static;
}

.cam-btn{
    color: #CCC;
    height: 54px;
    width: 200px;
    BACKGROUND: #648498;

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
  display: flex;

  align-items: baseline;
  width: 268px;
  height: 135px;
  top: 35px;
  left: 650px;
  position: absolute;
}

.box-3 .box-icon-cam {
  width: 23%;
}

.box-3 h3 {
    align-self: end;
    color:#ccc;
    position: absolute;
    left: 93px;
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
</style>
