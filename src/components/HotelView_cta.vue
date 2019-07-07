<template>
  <div class="cta">
    <h2 class="cta__book-now">
      Good news! We have 4 free rooms for your selected dates !
    </h2>
    <button class="btn">
      <span class="btn__visible">Book now</span>
      <span class="btn__invisible">Only 4 rooms left</span>
    </button>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
// Call to Action {
.cta {
  padding: 3.5rem 0;
  text-align: center;

  &__book-now {
    font-size: 2rem;
    font-weight: 300;
    text-transform: uppercase;
    margin-bottom: 2.5rem;
  }
}
// Button
.btn {
  font-size: 1.5rem;
  font-weight: 300;
  text-transform: uppercase;
  border-radius: 100px;
  border: none;
  background-image: linear-gradient(
    to right,
    var(--color-primary-light),
    var(--color-primary-dark)
  );
  color: #fff;
  position: relative;
  overflow: hidden;
  cursor: pointer;

  & > * {
    display: inline-block;
    height: 100%;
    width: 100%;
    transition: all 0.2s;
  }

  &__visible {
    padding: 2rem 7.5rem;
  }

  &__invisible {
    position: absolute;
    padding: 2rem 0;
    left: 0;
    top: -100%;
  }

  &:hover {
    background-image: linear-gradient(
      to left,
      var(--color-primary-light),
      var(--color-primary-dark)
    );
  }

  &:hover &__visible {
    transform: translateY(100%);
  }

  &:hover &__invisible {
    top: 0;
  }

  &:focus {
    outline: none;
    animation: pulsate 1s infinite;
  }
}
</style>
