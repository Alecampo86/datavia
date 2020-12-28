<template>
  <div class="netflix">
    <a href="#"
      ><img
        src="~assets/datavia-assets/datavia-assets/logo/datavia_logo_w.svg"
        alt=""
        class="datavia-logo"
    /></a>

    <!-- peliculas principal 2-->
    <!-- /////////////////////////////////////////////////////////////////////////////// -->

    <div class="row border border-danger rounded">
      <div class="col-lg-6 ">
        <div class="cam-name">
          <span>Camera Name</span>
          <h3>Camera c1 Out single loren ipsum cam</h3>
          <img class="temp-calib" src="~assets/datavia-assets/datavia-assets/icons/icon-temperature-calibration-active.svg" >
          <img class="measure-calib" src="~assets/datavia-assets/datavia-assets/icons/icon-measurement-calibration-active.svg" >
          <button type="button" class="cam-btn btn btn-info">Camera Setup</button>

        </div>
        <!-- imagen 1 -->
        <div class="bgcontainer">
          <div
            class="pelicula-principal border rounded"
            data-aos="fade-left"
            data-aos-duration="1000"

          ></div>
        </div>
        <!-- </div> -->
        <!-- imagen 2 CAMLOGO -->
        <div class="cam-logo">
          <img
            src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
          />
          <span class="cam-span text-white">Camera Setup</span>
        </div>
          <img class="grid-view" src="~assets/datavia-assets/datavia-assets/icons/icon-grid-view-active.svg" >
          <img class="list-view" src="~assets/datavia-assets/datavia-assets/icons/icon-list-view-active.svg" >

        <!-- imagen 3 PLANO -->
        <div class="cam-blueprint border rounded"
            data-aos="fade-left"
            data-aos-duration="1000"
             >

          <!-- <img
            src="~assets/datavia-assets/datavia-assets/images/big-map-example.jpg"
          /> -->
        </div>
        <span class="cam-location">Camera Location</span>
      </div>

      <div class="col-lg-6 ">
        <div class="container">
          <div class="peliculas-recomendadas contenedor">
            <div class="contenedor-titulo-controles text-center my-5">
              <input
                type="text"
                placeholder="Search cameras"
                class="cam-input form-control col-lg-12"
              />

              <div class="indicadores"></div>
            </div>

            <div class="contenedor-principal">
              <button
                role="button"
                id="flecha-izquierda"
                class="flecha-izquierda"
              >
                <i class="fas fa-angle-left"></i>
              </button>

              <div
                class="contenedor-carousel border rounded"
                data-aos="fade-right"
                data-aos-duration="1500"
              >
                <div class="carousel">
                  <div class="pelicula">
                    <a href="#"
                      ><img
                        src="~assets/images/cam-location-blueprint4.jpg"
                        alt=""
                    /></a>
                  </div>
                  <div class="pelicula">
                    <a href="#"
                      ><img src="~assets/images/cam-location-blueprint.jpg" alt=""
                    /></a>
                  </div>
                  <div class="pelicula">
                    <a href="#"
                      ><img src="~assets/images/cam-location-blueprint4.jpg" alt=""
                    /></a>
                  </div>
                  <div class="pelicula">
                    <a href="#"
                      ><img src="~assets/images/cam-location-blueprint2.jpg" alt=""
                    /></a>
                  </div>
                  <div class="pelicula">
                    <a href="#"
                      ><img
                        src="~assets/images/cam-location-blueprint4.jpg"
                        alt=""
                    /></a>
                  </div>
                </div>
              </div>

              <button role="button" id="flecha-derecha" class="flecha-derecha">
                <i class="fas fa-angle-right"></i>
              </button>
            </div>
          </div>
        </div>
      </div>

      <!-- /////////////////////////////////////////////////////////////////////////////// -->
    </div>
    <!-- <img
      src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
      class="slider-icon mx-3"
    />
    <img
      src="~assets/datavia-assets/datavia-assets/icons/icon-ai-sensing.svg"
      class="slider-icon mx-3"
    />
    <img
      src="~assets/datavia-assets/datavia-assets/icons/icon-dashboard-report.svg"
      class="slider-icon mx-3"
    /> -->

    <!-- peliculas recomendadas -->
    <div class="peliculas-recomendadas contenedor mt-5">
      <div class="contenedor-titulo-controles text-center my-2">
        <h3>Applications & Demos</h3>
        <div class="indicadores"></div>
      </div>

      <div class="contenedor-principal">
        <button role="button" id="flecha-izquierda" class="flecha-izquierda">
          <i class="fas fa-angle-left"></i>
        </button>

        <div
          class="contenedor-carousel"
          data-aos="fade-right"
          data-aos-duration="1500"
        >
          <div class="carousel">
            <div class="pelicula">
              <a href="#"
                ><img src="~assets/images/Biometric-identification.png" alt=""
              /></a>
            </div>
            <div class="pelicula">
              <a href="#"
                ><img src="~assets/images/cam-location-blueprint.jpg" alt=""
              /></a>
            </div>
            <div class="pelicula">
              <a href="#"
                ><img src="~assets/images/face-recog1.jpg" alt=""
              /></a>
            </div>
            <div class="pelicula">
              <a href="#"
                ><img src="~assets/images/face-recog3.jpg" alt=""
              /></a>
            </div>
            <div class="pelicula">
              <a href="#"
                ><img
                  src="~assets/images/facial-recognition-technologies-time-to-face-the-music_1500.jpg"
                  alt=""
              /></a>
            </div>
          </div>
        </div>

        <button role="button" id="flecha-derecha" class="flecha-derecha">
          <i class="fas fa-angle-right"></i>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "netflix",
  mounted() {
    AOS.init();
    const fila = document.querySelector(".contenedor-carousel");
    const peliculas = document.querySelectorAll(".pelicula");

    const flechaIzquierda = document.getElementById("flecha-izquierda");
    const flechaDerecha = document.getElementById("flecha-derecha");

    // ? ----- ----- Event Listener para la flecha derecha. ----- -----
    flechaDerecha.addEventListener("click", () => {
      fila.scrollLeft += fila.offsetWidth;

      const indicadorActivo = document.querySelector(".indicadores .activo");
      if (indicadorActivo.nextSibling) {
        indicadorActivo.nextSibling.classList.add("activo");
        indicadorActivo.classList.remove("activo");
      }
    });

    // ? ----- ----- Event Listener para la flecha izquierda. ----- -----
    flechaIzquierda.addEventListener("click", () => {
      fila.scrollLeft -= fila.offsetWidth;

      const indicadorActivo = document.querySelector(".indicadores .activo");
      if (indicadorActivo.previousSibling) {
        indicadorActivo.previousSibling.classList.add("activo");
        indicadorActivo.classList.remove("activo");
      }
    });

    // ? ----- ----- Paginacion ----- -----
    const numeroPaginas = Math.ceil(peliculas.length / 5);
    for (let i = 0; i < numeroPaginas; i++) {
      const indicador = document.createElement("button");

      if (i === 0) {
        indicador.classList.add("activo");
      }

      document.querySelector(".indicadores").appendChild(indicador);
      indicador.addEventListener("click", (e) => {
        fila.scrollLeft = i * fila.offsetWidth;

        document
          .querySelector(".indicadores .activo")
          .classList.remove("activo");
        e.target.classList.add("activo");
      });
    }

    // ? ----- ----- Hover ----- -----
    peliculas.forEach((pelicula) => {
      pelicula.addEventListener("mouseenter", (e) => {
        const elemento = e.currentTarget;
        setTimeout(() => {
          peliculas.forEach((pelicula) => pelicula.classList.remove("hover"));
          elemento.classList.add("hover");
        }, 300);
      });
    });

    fila.addEventListener("mouseleave", () => {
      peliculas.forEach((pelicula) => pelicula.classList.remove("hover"));
    });
  },
};
</script>

<style scoped>


.netflix{
  margin-top: 40px;
}
.pelicula-principal {

  font-size: 16px;
  height: 45%;
  color: #fff;
  background: linear-gradient(rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 100%),
    url(~assets/images/public-recog.jpg);
  background-position: center center;
  background-size: cover;
  margin-top: 0px;
  margin-bottom: 25px;
  cursor: pointer;
  width: 100%;
}



.bgcontainer {
  display: flex;
  flex-flow: row wrap;
  height: 660px;
}
.bgpic {
  position: absolute;
  top: 0;
  left: 340px;
  width: 400px;
  height: 260px;
}

.cam-logo {
  height: 100px;
  position: absolute;
  width: 306px;
  left: 60px;
  top: 435px;
  margin-top: 25px;
  margin-bottom: 25px;
  margin-left: 20px;
  border-bottom: white solid;

}

.cam-logo img {
    vertical-align: middle;
    border-style: none;
    position: absolute;
    top: 12px;
    left: -20px;
}



.cam-blueprint {
    position: absolute;
    top: 393px;
    left: 376px;
    width: 45%;
    height: 40%;
    background-size: cover;
    -webkit-transform: rotateX(45deg);
    transform: rotateX(45deg);
    margin-top: 25px;
    margin-bottom: 25px;
    margin-left: 10px;
    background-image: url(~assets/datavia-assets/datavia-assets/images/big-map-example.jpg);
    border: #11cdef;
}

.cam-blueprint img {
  height: 80%;
}

.cam-span{
    color: #fff !important;
    position: absolute;
    top: 97px;
    width: -12px;
    left: 0px;
}

.cam-location{
  color: #fff !important;
    position: absolute;
    top: 397px;
    width: -12px;
    left: 385px;

}

.cam-name{
    width: 100%;
    height: 50px;
    color: white;
    margin-top: 10px;
    margin-bottom: 10px;
}

.cam-name span{
  position: absolute;
    left: 16px;
    top: 15px;
}

.cam-name h3{

    color: #f5365c;
    font-weight: bold;
    position: absolute;
    top: 44px;
    left: 17px;
}

.temp-calib{
    position: absolute;
    top: 16px;
    left: 387px;
    cursor: pointer;
    transition: all 200ms;
}

.temp-calib:hover{
    position: absolute;
    top: 12px;
    left: 387px;
    cursor: pointer;

}

.measure-calib{
    position: absolute;
    top: 16px;
    right: 210px;
    cursor: pointer;
    transition: all 100ms;
}

.measure-calib:hover{
  position: absolute;
    top: 12px;
    right: 210px;
    cursor: pointer;
}

.cam-btn {
    position: absolute;
    top: 16px;
    right: 16px;
}

.grid-view  {
    position: absolute;
    bottom: 117x;
    left: 250px;
    top: 572px;
    cursor: pointer;
    transition: all 100ms;
}

.grid-view:hover  {
    position: absolute;

    left: 250px;
    top: 568px;
    cursor: pointer;
}

.list-view {
    position: absolute;
    cursor: pointer;
    bottom: 117px;
    left: 318px;
    transition: all 100ms;
}

.list-view:hover {
    position: absolute;
    cursor: pointer;
    bottom: 121px;
    left: 318px;
}

.cam-input{
  margin-top: -30px;
}
.pelicula-principal .contenedor {
  margin: 0 auto;
  margin-bottom: 6.25em;
  margin-top: 10px;
}

.pelicula-principal .titulo {
  font-weight: 600;
  font-size: 3.12em;
  margin-bottom: 0.4em;
}

.pelicula-principal .descripcion {
  font-weight: normal;
  font-size: 1em;
  line-height: 1.75em;
  max-width: 50%;
  margin-bottom: 1.25em;
}

.pelicula-principal .boton {
  background: rgba(0, 0, 0, 0.5);
  border: none;
  border-radius: 0.31em;
  padding: 0.93em 1.87em;
  color: #fff;
  margin-right: 1.25em;
  cursor: pointer;
  transition: 0.3s ease all;
  font-size: 1.12em;
}

.pelicula-principal .boton:hover {
  background: #fff;
  color: #000;
}

.pelicula-principal .boton i {
  margin-right: 1.25em;
}

/* ---- ----- ----- Contenedor Titulo y Controles ----- ----- ----- */
.contenedor-titulo-controles {
  display: flex;
  justify-content: space-between;
  flex: end;
}

.contenedor-titulo-controles h3 {
  color: #fff;
  font-size: 30px;
  margin: auto;
  margin-top: 10px;
  margin-bottom: 10px;
}

.contenedor-titulo-controles .indicadores button {
  background: #fff;
  height: 3px;
  width: 10px;
  cursor: pointer;
  border: none;
  margin-right: 2px;
}

.contenedor-titulo-controles .indicadores button:hover,
.contenedor-titulo-controles .indicadores button.activo {
  background: red;
}

/* ---- ----- ----- Contenedor Principal y Flechas ----- ----- ----- */
.peliculas-recomendadas {
  margin-bottom: 70px;
}

.peliculas-recomendadas .contenedor-principal {
  display: flex;
  align-items: center;
  position: relative;
}

.peliculas-recomendadas .contenedor-principal .flecha-izquierda,
.peliculas-recomendadas .contenedor-principal .flecha-derecha {
  position: absolute;
  border: none;
  background: rgba(0, 0, 0, 0.3);
  font-size: 40px;
  height: 50%;
  top: calc(50% - 25%);
  line-height: 40px;
  width: 50px;
  color: #fff;
  cursor: pointer;
  z-index: 500;
  transition: 0.2s ease all;
}

.peliculas-recomendadas .contenedor-principal .flecha-izquierda:hover,
.peliculas-recomendadas .contenedor-principal .flecha-derecha:hover {
  background: rgba(0, 0, 0, 0.9);
}

.peliculas-recomendadas .contenedor-principal .flecha-izquierda {
  left: 0;
}

.peliculas-recomendadas .contenedor-principal .flecha-derecha {
  right: 0;
}

/* ---- ----- ----- Carousel ----- ----- ----- */
.peliculas-recomendadas .contenedor-carousel {
  width: 100%;
  padding: 20px 0;
  overflow: hidden;
  scroll-behavior: smooth;
}

.peliculas-recomendadas .contenedor-carousel .carousel {
  display: flex;
  flex-wrap: nowrap;
}

.peliculas-recomendadas .contenedor-carousel .carousel .pelicula {
  min-width: 20%;
  transition: 0.3s ease all;
  box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.3);
}

.peliculas-recomendadas .contenedor-carousel .carousel .pelicula.hover {
  transform: scale(1.2);
  transform-origin: center;
  object-fit: cover;
}

.peliculas-recomendadas .contenedor-carousel .carousel .pelicula img {
  width: 100%;
  vertical-align: top;
  object-fit: cover;
  height: 100%;
}

/* ---- ----- ----- Media Queries ----- ----- ----- */
@media screen and (max-width: 800px) {
  header .logotipo {
    margin-bottom: 10px;
    font-size: 30px;
  }

  header .contenedor {
    flex-direction: column;
    text-align: center;
  }

  .pelicula-principal {
    font-size: 14px;
  }

  .pelicula-principal .descripcion {
    max-width: 100%;
  }

  .peliculas-recomendadas .contenedor-carousel {
    overflow: visible;
  }

  .peliculas-recomendadas .contenedor-carousel .carousel {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
  }

  .peliculas-recomendadas .indicadores,
  .peliculas-recomendadas .flecha-izquierda,
  .peliculas-recomendadas .flecha-derecha {
    display: none;
  }
}
</style>
