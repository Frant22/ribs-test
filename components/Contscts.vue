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
    position: absolute;
    top: 60px;
    right: 80px;
    display: flex;
    gap: 20px;

    &__text {
      position: relative;
      color: #CD1212;
      font-size: 42px;

      &::after {
        content: "";
        position: absolute;
        bottom: 20px;
        left: 0;
        width: 290px;
        height: 1px;
        background-color: #CD1212;
      }
    }

    &__button {
      width: 90px;
      height: 90px;

      color: #CD1212;
      font-size: 40px;

      border: none;
      background: rgba(196, 196, 196, 0.13);
      border-radius: 50%;
      }

    &__underline {
      width: 1700px;
      height: 70px;
      border-bottom: 1px solid rgba(200, 200, 200, 0.46);;
    }
  }
</style>
