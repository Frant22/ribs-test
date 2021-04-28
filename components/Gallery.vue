<template>
  <div class="gallery">
    <div class="gallery__buttons">
      <button class="button gallery__buttons gallery__buttons-top" />
      <button class="button gallery__buttons gallery__buttons-bottom" />
    </div>

    <div class="gallery__content">
      <div class="gallery__content gallery__content-top">
        <div class="bar">
          <span>&#8544;.</span>
          <span>&#8545;</span>
          <span>&#8546;</span>
          <span>&#8547;</span>
        </div>
        <div class="project-number">
          <strong>S047</strong> Project
        </div>
      </div>
      <div class="gallery__picture" />
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

    padding-right: 80px;

    &__buttons {
      display: flex;
      flex-direction: column;
      gap: 30px;

      &-bottom {
        width: 100px;
        height: 100px;
        background: url('~/static/icons/arrow.svg') no-repeat center;
        border-radius: 50%;
        border: 1px solid #C8C8C8;
        transform: rotate(180deg);
      }

      &-top {
        width: 100px;
        height: 100px;
        background: url('~/static/icons/arrow.svg') no-repeat center;
        border-radius: 50%;
        border: 1px solid #C8C8C8;
      }
    }

    &__content {
      display: flex;
      flex-direction: column;
      width: 1000px;

      &-top {
        flex-direction: row;
        justify-content: space-between;
      }
    }
  }
</style>
