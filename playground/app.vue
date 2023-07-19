<template>
  <CCarousel>
    <CSlide v-for="slide in 10" :key="slide">
      <div class="carousel__item">
        {{ slide }}
      </div>
    </CSlide>

    <template #addons>
      <CNavigation />
      <CPagination />
    </template>
  </CCarousel>
</template>

<style>
.carousel__item {
  background-color: rgb(134, 239, 172);
  color: white;
  min-height: 200px;
  width: 100%;
  font-size: 20px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.carousel__slide {
  padding: 10px;
}

.carousel__prev,
.carousel__next {
  box-sizing: content-box;
  border: 5px solid white;
}
</style>