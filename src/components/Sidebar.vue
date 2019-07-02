<template>
  <nav class="sidebar">
    <ul class="side-nav">
      <li class="side-nav__item">
        <a href="#" class="side-nav__link">
          <svg class="side-nav__icon">
            <use xlink:href="../assets/img/sprite.svg#icon-home"></use>
          </svg>
          <span>Hotel</span>
        </a>
      </li>

      <li>
        <a href="#" class="side-nav__link">
          <svg class="side-nav__icon">
            <use
              xlink:href="../assets/img/sprite.svg#icon-aircraft-take-off"
            ></use>
          </svg>
          <span>Flight</span>
        </a>
      </li>

      <li>
        <a href="#" class="side-nav__link">
          <svg class="side-nav__icon">
            <use xlink:href="../assets/img/sprite.svg#icon-key"></use>
          </svg>
          <span>Car rental</span>
        </a>
      </li>

      <li>
        <a href="#" class="side-nav__link">
          <svg class="side-nav__icon">
            <use xlink:href="../assets/img/sprite.svg#icon-map"></use>
          </svg>
          <span>Tours</span>
        </a>
      </li>
    </ul>

    <div class="legal">&copy; {{ year }} by trillo. All rights reserved.</div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>

<style lang="scss"></style>
