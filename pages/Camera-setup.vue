<template>
  <div>
    <!--Header-->
    <div class="header pt-5 pb-7">
      <div class="container">
        <div class="header-body">
          <section class="py-6 pb-9">

            <div class="row justify-content-center text-center">
              <div class="col-md-9">
                <h1>CAMERA</h1>
                <netflix />
              </div>
            </div>
          </section>
        </div>
      </div>

      <!-- /////////////////SEPARADOR ///////////////////////-->
      <div class="separator separator-bottom separator-skew zindex-100">
        <svg
          x="0"
          y="0"
          viewBox="0 0 2560 100"
          preserveAspectRatio="none"
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
        >
          <polygon
            class="fill-default"
            points="2560 0 2560 100 0 100"
          ></polygon>
        </svg>
      </div>
    </div>

    <!-- SECCION 2 -->
  </div>
</template>

<script>
import Netflix from "../pages/Netflix.vue";

export default {
  components: { Netflix },
  layout: "AuthLayout",
};
</script>




<style>
</style>
