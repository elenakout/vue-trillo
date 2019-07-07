<template>
  <div class="main-header">
    <header class="header">
      <img src="../assets/img/logo.png" alt="trillo logo" class="logo" />
      <form action="#" class="search">
        <input type="text" class="search__input" placeholder="Search hotels" />
        <button class="search__button">
          <svg class="search__icon">
            <use
              xlink:href="../assets/img/sprite.svg#icon-magnifying-glass"
            ></use>
          </svg>
        </button>
      </form>

      <nav class="user-nav">
        <div class="user-nav__icon-box">
          <svg class="user-nav__icon">
            <use xlink:href="../assets/img/sprite.svg#icon-bookmark"></use>
          </svg>
          <span class="user-nav__notification">7</span>
        </div>

        <div class="user-nav__icon-box">
          <svg class="user-nav__icon">
            <use xlink:href="../assets/img/sprite.svg#icon-chat"></use>
          </svg>
          <span class="user-nav__notification">13</span>
        </div>

        <div class="user-nav__user">
          <img src="../assets/img/user.jpg" class="user-nav__user-photo" />
          <span class="user-nav__user-name">Jonas</span>
        </div>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style lang="scss">
// LOGO

.logo {
  height: 3.25rem;
  margin-left: 2rem;
}

// SEARCH
.search {
  flex: 0 0 40%;

  display: flex;
  align-items: center;
  justify-content: center;

  &__input {
    font-family: inherit;
    font-size: inherit;
    color: inherit;
    background-color: var(--color-grey-light-2);
    border: none;
    padding: 0.7rem 2rem;
    border-radius: 100px;
    width: 90%;
    transition: all 0.2s;
    margin-right: -3.25rem;

    &:focus {
      outline: none;
      width: 100%;
      background-color: var(--color-grey-light-3);
    }

    &::-webkit-input-placeholder {
      font-weight: 100;
      color: var(--color-grey-dark-3);
    }
  }

  &__input:focus + &__button {
    background-color: var(--color-grey-light-3);
  }

  &__button {
    border: none;
    background-color: var(--color-grey-light-2);

    &:focus {
      outline: none;
    }

    &:active {
      transform: translateY(2px);
    }
  }

  &__icon {
    height: 2rem;
    width: 2rem;
    fill: var(--color-grey-dark-3);
  }
}

// USER NAVIGATION
.user-nav {
  display: flex;
  align-items: center;
  align-self: stretch;

  & > * {
    padding: 0 2rem;
    cursor: pointer;
    height: 100%;
    display: flex;
    align-items: center;
  }

  & > *:hover {
    background-color: var(--color-grey-light-2);
  }

  &__icon-box {
    position: relative;
  }

  &__icon {
    height: 2.25rem;
    width: 2.25rem;
    fill: var(--color-grey-dark-2);
  }

  &__notification {
    font-size: 0.8rem;
    height: 1.75rem;
    width: 1.75rem;
    border-radius: 50%;
    background-color: var(--color-primary);
    color: #fff;
    position: absolute;
    top: 1.5rem;
    right: 1.1rem;

    display: flex;
    justify-content: center;
    align-items: center;
  }

  &__user-photo {
    height: 3.75rem;
    border-radius: 50%;
    margin-right: 1rem;
  }
}
</style>
