<template>
  <div class="container">
    <h1>AOS ANIMATION</h1>

     <div class="container">
<!------------------------------------------------------------>
          <div class="div">
            I am div 1
          </div>
<!--------------------------------------------------------------->
          <div class="div" data-aos="fade-left" data-aos-duration="1000" data-aos-once="true">
            I am div 2
          </div>
<!-------------------------------------------------------------->
          <div class="div" data-aos="fade-right">
            I am div 3
          </div>
<!-- ------------------------------------------------------------->
          <div class="div"  data-aos="fade-up">
            I am div 4
          </div>
<!-- ------------------------------------------------------------->
          <div class="div"  data-aos="zoom-in">
            I am div 5
          </div>
<!-- ------------------------------------------------------------->
          <div class="div" data-aos="flip-up">
            I am div 6
          </div>
<!-- ------------------------------------------------------------->
    </div>
  </div>
</template>

<script>

export default {
mounted(){

   AOS.init();
}
}
</script>

<style scoped>
*{
  margin: 0;
  padding: 0;
}
body{
  font-size: 30px;
  font-family: sans-serif;
  background: #ebebeb;
}
.container{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  flex-direction: column;
}
.div{
   box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.2);
  height: 300px;
  width: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(to right, #1cd8d2, #93edc7);
  color: white;
  margin: 100px 0;
  border-radius: 7px;
}


</style>
