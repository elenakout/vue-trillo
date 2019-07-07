<template>
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
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
// Hotel Overview

.overview {
  display: flex;
  align-items: center;
  border-bottom: 1px solid var(--color-grey-light-2);

  &__heading {
    font-size: 2.25rem;
    font-weight: 300;
    text-transform: uppercase;
    letter-spacing: 1px;
    padding: 1.5rem 3rem;
  }

  &__stars {
    margin-right: auto;
    display: flex;
  }

  &__icon-star,
  &__icon-location {
    width: 1.75rem;
    height: 1.75rem;
    fill: var(--color-primary);
  }

  &__location {
    font-size: 1.2rem;
    display: flex;
    align-items: center;
  }

  &__icon-location {
    margin-right: 0.5rem;
  }

  &__rating {
    background-color: var(--color-primary);
    color: #fff;
    margin-left: 3rem;
    padding: 0 2.25rem;
    align-self: stretch;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  &__rating-average {
    font-size: 2.25rem;
    font-weight: 300;
    margin-bottom: -3px;
  }

  &__rating-count {
    font-size: 0.8rem;
    text-transform: uppercase;
  }
}
</style>
