<template>
  <section id="background">
    <div class="box-3">
      <img
        class="box-icon-cam"
        src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
      />
      <h2 class="text-white ml-2">Camera Management</h2>
    </div>

    <!-- ////////////////////////icono home///////////////// -->
    <div class="container row">
      <nuxt-link to="/">
        <div class="icon-menu">
          <div class="logo">
            <img
              src="~assets/datavia-assets/datavia-assets/icons/icon-home.svg"
              alt=""
            />
            <small>MENU</small>
          </div>
        </div>
      </nuxt-link>
      <!-- COLUMNA 1 -->
      <div class="columna1 col col-lg-6 h-100 w-100">

        <div class="column-title w-75">
          <i class="file fas fa-file-alt"></i>
          <h2 class="text-white mt-1">Added Camera Description</h2>
        </div>


        <input
          type="text"
          placeholder="Camera A1 - Building R1 - Floor 1 A"
          class="cam-name form-control mt-3 w-75 p-2 bg-dark"
        />



        <div class="rowSelect row w-100">
            <input
            type="select"
            class="select1 form-control bg-dark mt-3 col-4 p-2"
            placeholder="Sony"
          />
          <input
            type="select"
            class="select2 form-control bg-dark mt-3 col-4 p-2"
            placeholder="ABC100"
          />
        </div>

        <div class="columnaBox w-75 h-25 mt-5">
          <img src="~assets/datavia-assets/datavia-assets/images/camera.png" />
        </div>

        <div class="form-group">
          <textarea class="cam-description bg-dark form-control p-2" rows="3">
Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias, sunt? Mollitia, rem aliquam consequatur laudantium sapiente doloremque, ducimus possimus in dignissimos fugit aut adipisci consectetur sequi atque, tempora tenetur corporis?</textarea
          >
        </div>
      </div>

      <!-- COLUMNA 2 -->
      <div class="columna2 col col-lg-6 h-100 w-100">
        <div class="column-title w-75">
          <i class="fas fa-map-marker-alt"></i>

          <h2 class="text-white mt-1">Associate Camera to Location</h2>
        </div>



        <div class="columnaBox3 w-100 mt-5">

          <nuxt-link to="/flat">
            <button class="btn flat-btn">
              <img class="gear fas fa-cog "
                  src="~assets/datavia-assets/datavia-assets/icons/icon-setup.svg"/>
                  <span>Add Flat</span>

            </button>
          </nuxt-link>
        </div>

        <div>
          <button class="btn cancel-btn">
            <i class="far fa-window-close"></i>
            <span>Cancel</span>
          </button>
        </div>

        <div class="save-continue">
          <nuxt-link to="/camera-save">
            <button class="btn save-btn">
              <img
                class="icon-save"
                src="~assets/datavia-assets/datavia-assets/icons/icon-save.svg"
              /><span>Save and Continue</span>
            </button>
          </nuxt-link>
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

.cancel-btn {
  color: black;
  height: 35px;
  width: 130px;
  background: #85b0cb;
  position: absolute;
  bottom: 55px;
  left: 170px;
  width: 120px;
  border-radius: 5px;
  -webkit-transition: all 100ms;
  transition: all 100ms;
  font-size: 12px;
}

.cancel-btn i {
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
.save-btn {
  color: black;
  height: 35px;

  background: #85b0cb;
  position: absolute;
  bottom: 55px;
  left: 312px;
  width: 170px;
  border-radius: 5px;
  -webkit-transition: all 100ms;
  transition: all 100ms;
  font-size: 12px;
}

.flat-btn{

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

.columnaBox3 img{

    object-fit: initial;
    width: 16%;
    position: absolute;
    left: 18px;
    top: 7px;
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

.cam-name{
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
.cam-name{
    position: absolute;
    top: 204px;
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
  border-radius: 10px;
  position: absolute;
  top: -86px;
  left: 0px;
  transition: all 200ms;
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

.file{
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
  justify-content: end;
  flex-flow: column wrap;
}

.columna2 {
  display: flex;
  align-items: center;
  justify-content: end;
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

.columnaBox3 {
  display: flex;
  align-items: center;
  justify-content: center;
  align-self: initial;
  position: absolute;
  top: 0px;
  height: 441px;
  border: solid #85b0cb;
  border-style: dotted;
  border-radius: 10px;
  cursor: pointer;
  object-fit: cover;
}

.fa-map-marker-alt:before {
    content: "\f3c5";
    position: absolute;
    left: -70px;
}


</style>
