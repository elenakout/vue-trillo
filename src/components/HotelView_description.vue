<template>
  <div class="detail">
    <div class="description">
      <p class="paragraph">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem
        repellat itaque dolorem, aliquid dolorum sit dolores illum minima
        numquam harum animi tempora voluptatem optio! Tenetur?
      </p>
      <p class="paragraph">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur,
        possimus saepe! Vel blanditiis debitis laborum.
      </p>
      <ul class="list">
        <li class="list__item">Close to the beach</li>
        <li class="list__item">Breakfast included</li>
        <li class="list__item">Free airport shuttle</li>
        <li class="list__item">Free wifi in all rooms</li>
        <li class="list__item">Air condition and heating</li>
        <li class="list__item">Pets allowed</li>
        <li class="list__item">We speak all languages</li>
        <li class="list__item">Perfect for families</li>
      </ul>
      <div class="recommend">
        <p class="recommend__count">
          Lucy and 3 other friends recommend this hotel.
        </p>
        <div class="recommend__friends">
          <img
            src="../assets/img/user-3.jpg"
            alt="Friend 1"
            class="recommend__photo"
          />
          <img
            src="../assets/img/user-4.jpg"
            alt="Friend 2"
            class="recommend__photo"
          />
          <img
            src="../assets/img/user-5.jpg"
            alt="Friend 3"
            class="recommend__photo"
          />
          <img
            src="../assets/img/user-6.jpg"
            alt="Friend 4"
            class="recommend__photo"
          />
        </div>
      </div>
    </div>
    <div class="user-reviews">
      user-reviews
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.detail {
  display: flex;
  padding: 4.5rem;
  background-color: var(--color-grey-light-1);
  border-bottom: var(--line);
}

.description {
  font-size: 1.4rem;
  background-color: #fff;
  box-shadow: var(--shadow-light);
  padding: 3rem;
  flex: 0 0 60%;
  margin-right: 4.5rem;
}

.user-reviews {
  background-color: yellowgreen;
  flex: 1;
}

.recommend {
  font-size: 1.3rem;
  color: var(--color-grey-dark-3);

  display: flex;
  //justify-content: space-between;
  align-items: center;

  &__count {
    margin-right: auto;
  }

  &__friends {
  }

  &__photo {
    box-sizing: content-box;
    border: solid 0.3rem #fff;
    height: 4rem;
    width: 4rem;
    border-radius: 50%;

    &:not(:last-child) {
      margin-right: -1.5rem;
    }
  }
}
</style>
