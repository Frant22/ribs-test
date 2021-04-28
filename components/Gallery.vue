<template>
  <div class="gallery">
    <div class="gallery__navigation">
      <div class="gallery__buttons">
        <button class="button gallery__buttons gallery__buttons-top" />
        <button class="button gallery__buttons gallery__buttons-bottom" />
      </div>
      <ul class="list">
        <li class="list__item list__item-visible">
          En
        </li>
        <li class="list__item">
          Ru
        </li>
        <li class="list__item">
          Ua
        </li>
      </ul>
      <ul class="list menu gallery__menu">
        <li>
          <a class="menu__element" href="#">
            Home
          </a>
        </li>
        <li>
          <a class="menu__element" href="#">
            Project<span class="decoration">.52</span>
          </a>
        </li>
        <li>
          <a class="menu__element" href="#">
            About
          </a>
        </li>
        <li>
          <a class="menu__element" href="#">
            Services
          </a>
        </li>
        <li>
          <a class="menu__element" href="#">
            Contact
          </a>
        </li>
      </ul>
    </div>

    <div class="gallery__content">
      <div class="gallery__content gallery__content-top">
        <div class="bar">
          <span class="bar__item bar__item-active">l.</span>
          <span class="bar__item">ll</span>
          <span class="bar__item">lll</span>
          <span class="bar__item">lV</span>
        </div>
        <div class="gallery__title">
          <span class="gallery__title gallery__title-number">
            S047
          </span>
          Project
        </div>
      </div>

      <ul class="list">
        <li class="gallery__picture gallery__picture-active" />
        <li>
          <img class="gallery__picture" src="" alt="">
        </li>
        <li>
          <img class="gallery__picture" src="" alt="">
        </li>
        <li>
          <img class="gallery__picture" src="" alt="">
        </li>
      </ul>
      <button class="button gallery__button">
        OPEN PROJECT
      </button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
  .gallery {
    display: flex;
    justify-content: space-between;
    width: 90vw;

    &__navigation {
      display: flex;
      flex-direction: column;
      gap: 8rem;
    }

    &__buttons {
      display: flex;
      flex-direction: column;
      gap: 2rem;

      padding-top: 2rem;

      &-bottom {
        width: 70px;
        height: 70px;
        background: url('~/static/icons/arrow.svg') no-repeat center;
        border-radius: 50%;
        border: 1px solid #C8C8C8;
        transform: rotate(180deg);
      }

      &-top {
        width: 4.4rem;
        height: 4.4rem;
        background: url('~/static/icons/arrow.svg') no-repeat center;
        border-radius: 50%;
        border: 1px solid #C8C8C8;
      }
    }

    &__content {
      position: relative;
      display: flex;
      flex-direction: column;
      width: 62.5rem;
      gap: 2rem;

      &-top {
        flex-direction: row;
        justify-content: space-between;
        align-items: flex-end;
      }
    }

    &__title {
      font-size: 1.5rem;
      line-height: 1;

      &-number {
        font-size: 4rem;
      }
    }

    &__picture {
      background: url('~/static/images/picture-1.png') no-repeat center;
      width: 62.5rem;
      height: 33.8rem;
      background-size: contain;

      display: none;

      &-active {
        display: block;
      }
    }

    &__button {
      position: absolute;
      bottom: 0;
      right: 0;

      width: 14rem;
      height: 7rem;
      color: white;
      background-color: #CD1212;
      border: none;

      &::after {
        content: "";
        background-color: white;
        width: 2rem;
        height: 1px;

        position: absolute;
        bottom: 2.5rem;
        left: 3.8rem;

        transition: width 0.5s ease;
      }

      &:hover {
        &::after {
          width: 6.5rem;
        }
      }
    }
  }
</style>
