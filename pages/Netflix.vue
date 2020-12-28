<template>
  <div class="netflix">
    <!-- <a href="#"
      ><img
        src="~assets/datavia-assets/datavia-assets/logo/datavia_logo_w.svg"
        alt=""
        class="datavia-logo"
    /></a> -->

    <!-- peliculas principal 2-->
    <!-- /////////////////////////////////////////////////////////////////////////////// -->

    <div class="row">
      <div class="col-lg-6 bgcontainer border">
        <!-- <div class="container bgpic"> -->
        <!-- imagen 1 -->
        <div
          class="pelicula-principal"
          data-aos="fade-left"
          data-aos-duration="1000"
          data-aos-once="true"
        ></div>
        <!-- </div> -->
        <!-- imagen 2 CAMLOGO -->
        <div class="cam-logo">
          <img
            src="~assets/datavia-assets/datavia-assets/icons/icon-camera-setup.svg"
          />
          <span class="cam-span text-white">CAMERA SETUP</span>
        </div>
        <!-- imagen 3 PLANO -->
        <div class="cam-blueprint">

          <!-- <img
            src="~assets/datavia-assets/datavia-assets/images/big-map-example.jpg"
          /> -->
        </div>
        <span class="cam-location">CAMERA LOCATION</span>
      </div>

      <div class="col-lg-6 border">
        <div class="container">
          <div class="peliculas-recomendadas contenedor">
            <div class="contenedor-titulo-controles text-center my-5">
              <input
                type="text"
                placeholder="Search cameras"
                class="form-control col-lg-12"
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
                class="contenedor-carousel"
                data-aos="fade-right"
                data-aos-duration="1500"
              >
                <div class="carousel">
                  <div class="pelicula">
                    <a href="#"
                      ><img
                        src="~assets/images/Biometric-identification.png"
                        alt=""
                    /></a>
                  </div>
                  <div class="pelicula">
                    <a href="#"
                      ><img src="~assets/images/face-recog2.jpg" alt=""
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
    <div class="peliculas-recomendadas contenedor">
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
                ><img src="~assets/images/face-recog2.jpg" alt=""
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
/* ---- ----- ----- Pelicula Principal ----- ----- ----- */
.pelicula-principal {
  border-top: solid;
  border-bottom: solid;
  font-size: 16px;
  height: 45%;
  color: #fff;
  background: linear-gradient(rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 100%),
    url(~assets/images/public-recog.jpg);
  background-position: center center;
  background-size: cover;
  margin-top: 25px;
  margin-bottom: 25px;

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
  width: 200px;
  left: 60px;
  top: 435px;
  margin-top: 25px;
  margin-bottom: 25px;
  margin-left: 20px;
  border-bottom: white solid;
  border-top: white solid;
}

.cam-logo img {
    vertical-align: middle;
    border-style: none;
    position: absolute;
    top: 12px;
    left: 50px;
}



.cam-blueprint {
    position: absolute;
    top: 295px;
    left: 376px;
    width: 45%;
    height: 57%;
    background-size: cover;
    -webkit-transform: rotateX(45deg);
    transform: rotateX(45deg);
    margin-top: 25px;
    margin-bottom: 25px;
    margin-left: 10px;
    background-image: url(~assets/datavia-assets/datavia-assets/images/big-map-example.jpg);
    border-top: white solid;
    border-bottom: white solid;
}

.cam-blueprint img {
  height: 80%;
}

.cam-span{

    color: #fff !important;
    position: absolute;
    top: 105px;
    width: -12px;
    left: 47px;
}

.cam-location{
  color: #fff !important;
    position: absolute;
    top: 350px;
    width: -12px;
    left: 385px;

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
