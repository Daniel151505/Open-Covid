<template>

  <div>
  <section id="slider">
    <div id="sliderCarousel" data-bs-interval="5000" class="carousel sslider carousel-fade" data-bs-ride="carousel">

      <ol class="carousel-indicators" id="slider-carousel-indicators"></ol>

      <div class="carousel-inner" role="listbox">
        <div class="carousel-item active">
        </div>
      </div>
    </div>
  </section>
  </div>
</template>

<script>
export default {

}
</script>

<style>

/*--Slider--*/

#slider {
  width: 100%;
  height: 100vh;
  background-color: rgba(60, 60, 60, 0.8);
  overflow: hidden;
  position: relative;
}

#slider .carousel, #slider .carousel-inner, #slider .carousel-item, #slider .carousel-item::before {
  position: absolute;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
}

#slider .carousel-item {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  background-image: url(../assets/slide/slide-1.jpg);
}

@media (max-width: 1200px) {
  #slider .container {
    margin-left: 50px;
    margin-right: 50px;
  }
}

#slider h2 {
  color: #2f2f2f;
  margin-bottom: 20px;
  font-size: 36px;
  font-weight: 700;
}

#slider p {
  margin: 0 auto 30px auto;
  color: #555555;
}

#slider .carousel-inner .carousel-item {
  transition-property: opacity;
  background-position: center top;
}

#slider .carousel-inner .carousel-item,
#slider .carousel-inner .active.carousel-item-start,
#slider .carousel-inner .active.carousel-item-end {
  opacity: 0;
}

#slider .carousel-inner .active,
#slider .carousel-inner .carousel-item-next.carousel-item-start,
#slider .carousel-inner .carousel-item-prev.carousel-item-end {
  opacity: 1;
  transition: 0.5s;
}

#slider .carousel-inner .carousel-item-next,
#slider .carousel-inner .carousel-item-prev,
#slider .carousel-inner .active.carousel-item-start,
#slider .carousel-inner .active.carousel-item-end {
  left: 0;
  transform: translate3d(0, 0, 0);
}

#slider .carousel-indicators li {
  cursor: pointer;
  background: #fff;
  overflow: hidden;
  border: 0;
  width: 12px;
  height: 12px;
  border-radius: 50px;
  opacity: .6;
  transition: 0.3s;
}

@media (max-width: 992px) {
  #slider {
    height: 100vh;
  }
  #slider .container {
    margin-top: 100px;
  }
}

@media (max-width: 768px) {
  #slider h2 {
    font-size: 28px;
  }
}

@media (min-width: 1024px) {
  #slider .carousel-control-prev, #slider .carousel-control-next {
    width: 5%;
  }
}

@media (max-height: 500px) {
  #slider {
    height: 160vh;
  }
}
</style>