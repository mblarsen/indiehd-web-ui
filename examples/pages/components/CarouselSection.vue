<template>
  <div class="section" id="carousel">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-8">
          <el-carousel height="500px">
            <el-carousel-item class="carousel-item">
              <img alt="First slide" class="d-block" src="img/bg1.jpg">
              <div class="carousel-caption d-none d-md-block">
                <h5>Nature, United States</h5>
              </div>
            </el-carousel-item>
            <el-carousel-item class="carousel-item">
              <img alt="Second slide" class="d-block" src="img/bg3.jpg">
              <div class="carousel-caption d-none d-md-block">
                <h5>Somewhere Beyond, United States</h5>
              </div>
            </el-carousel-item>
            <el-carousel-item class="carousel-item">
              <img alt="Third slide" class="d-block" src="img/bg4.jpg">
              <div class="carousel-caption d-none d-md-block">
                <h5>Yellowstone National Park, United States</h5>
              </div>
            </el-carousel-item>
          </el-carousel>
        </div>
      </div>
    </div>
  </div>

</template>
<script>
  import { Carousel, CarouselItem } from 'element-ui';

  export default {
    components: {
      [Carousel.name]: Carousel,
      [CarouselItem.name]: CarouselItem
    }
  };
</script>
<style>
</style>
