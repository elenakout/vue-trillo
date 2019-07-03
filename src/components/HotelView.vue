<template>
  <main class="hotel-view">
    <div class="gallery">
      <figure class="gallery__item">
        <img
          src="../assets/img/hotel-1.jpg"
          alt="Hotel photo 1"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__item">
        <img
          src="../assets/img/hotel-2.jpg"
          alt="Hotel photo 3"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__item">
        <img
          src="../assets/img/hotel-3.jpg"
          alt="Hotel photo 3"
          class="gallery__photo"
        />
      </figure>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
// Gallery
.gallery {
  display: flex;

  &__photo {
    width: 100%;
    display: block;
  }
}
</style>
