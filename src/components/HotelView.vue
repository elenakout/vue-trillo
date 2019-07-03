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

    <div class="overview">
      <h1 class="overview__heading">
        Hotel Las Palmas
      </h1>
      <div class="overview__stars">
        <svg class="overview__icon-star">
          <use xlink:href="../assets/img/sprite.svg#icon-star"></use>
        </svg>
        <svg class="overview__icon-star">
          <use xlink:href="../assets/img/sprite.svg#icon-star"></use>
        </svg>
        <svg class="overview__icon-star">
          <use xlink:href="../assets/img/sprite.svg#icon-star"></use>
        </svg>
        <svg class="overview__icon-star">
          <use xlink:href="../assets/img/sprite.svg#icon-star"></use>
        </svg>
        <svg class="overview__icon-star">
          <use xlink:href="../assets/img/sprite.svg#icon-star"></use>
        </svg>
      </div>
      <div class="overview__location">
        <svg class="overview__icon-location">
          <use xlink:href="../assets/img/sprite.svg#icon-location-pin"></use>
        </svg>
        <button class="btn-inline">Albufeira, Portugal</button>
      </div>

      <div class="overview__rating">
        <div class="overview__rating-average">8.6</div>
        <div class="overview__rating-count">429 votes</div>
      </div>
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

// Hotel Overview

.overview {
  display: flex;

  &__heading {
  }

  &__stars {
    margin-right: auto;
  }

  &__icon-star,
  &__icon-location {
    width: 1.75rem;
    height: 1.75rem;
    fill: var(--color-primary);
  }

  &__location {
  }

  &__rating {
  }

  &__rating-average {
  }

  &__rating-count {
  }
}
</style>
