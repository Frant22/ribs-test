<template>
  <div class="contacts">
    <span class="contacts__text">
      GET IN TOUCH
    </span>
    <button class="contacts__button">
      &#x2b;
    </button>
    <span class="contacts__underline" />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
  .contacts {
    // position: absolute;
    // top: 3rem;
    // right: 6rem;
    display: flex;
    justify-content: flex-end;
    gap: 1.2rem;

    &__text {
      position: relative;
      color: #CD1212;
      font-size: 1rem;

      &::after {
        content: "";
        position: absolute;
        bottom: 0.9rem;
        left: 0;
        width: 7rem;
        height: 1px;
        background-color: #CD1212;
      }
    }

    &__button {
      width: 2.5rem;
      height: 2.5rem;

      color: #CD1212;
      font-size: 1.5rem;

      border: none;
      background: rgba(196, 196, 196, 0.13);
      border-radius: 50%;
      }

    &__underline {
      width: 49.5rem;
      height: 1.7rem;
      border-bottom: 1px solid rgba(200, 200, 200, 0.46);;
    }
  }
</style>
