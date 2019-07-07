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
      <figure class="review">
        <blockquote class="review__text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga animi
          dignissimos impedit excepturi reiciendis totam.
        </blockquote>
        <figcaption class="review__user">
          <img
            src="../assets/img/user-1.jpg"
            alt="User 1"
            class="review__photo"
          />
          <div class="review__user-box">
            <p class="review__user-name">Nick Smith</p>
            <p class="review__user-date">Feb 23rd, 2019</p>
          </div>
          <div class="review__rating">7.8</div>
        </figcaption>
      </figure>

      <figure class="review">
        <blockquote class="review__text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Eos a omnis
          libero.
        </blockquote>
        <figcaption class="review__user">
          <img
            src="../assets/img/user-2.jpg"
            alt="User 2"
            class="review__photo"
          />
          <div class="review__user-box">
            <p class="review__user-name">Jane Doe</p>
            <p class="review__user-date">Jun 4th, 2019</p>
          </div>
          <div class="review__rating">9.3</div>
        </figcaption>
      </figure>
      <button class="btn-inline">Show all <span>&rarr;</span></button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.detail {
  font-size: 1.4rem;
  display: flex;
  padding: 4.5rem;
  background-color: var(--color-grey-light-1);
  border-bottom: var(--line);
}

.description {
  background-color: #fff;
  box-shadow: var(--shadow-light);
  padding: 3rem;
  flex: 0 0 60%;
  margin-right: 4.5rem;
}

.user-reviews {
  flex: 1;

  display: flex;
  flex-direction: column;
  align-items: center;
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

// REVIEWS
.review {
  background-color: #fff;
  box-shadow: var(--shadow-light);
  padding: 3rem;
  margin-bottom: 2rem;
  position: relative;
  overflow: hidden;

  &__text {
    margin-bottom: 3rem;
    z-index: 10;
    position: relative;
  }

  &__user {
    display: flex;
    align-items: center;
  }

  &__photo {
    height: 4.5rem;
    width: 4.5rem;
    border-radius: 50%;
    margin-right: 1.5rem;
  }

  &__user-box {
    margin-right: auto;
  }

  &__user-name {
    font-size: 1.1rem;
    text-transform: uppercase;
    font-weight: 600;
    margin-bottom: 0.4rem;
  }

  &__user-date {
    font-size: 1rem;
    color: var(--color-grey-dark-3);
  }

  &__rating {
    font-size: 2.2rem;
    color: var(--color-primary);
    font-weight: 300;
  }

  &::before {
    content: "\201C";
    position: absolute;
    top: -2.75rem;
    left: -1rem;
    line-height: 1;
    font-size: 20rem;
    color: var(--color-grey-light-2);
    font-family: sans-serif;
    z-index: 1;
  }
}
</style>
