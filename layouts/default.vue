<template>
  <div>
    <Nuxt />
  </div>
</template>

<style lang='scss'>
html {
  font-family: 'Favorit Trial Std',
    'Source Sans Pro',
    'Segoe UI',
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

a {
  color: black;
  text-decoration: none;
}

.button {
  cursor: pointer;
}

.bar {
  display: flex;
  gap: 5.6rem;

  &__item {
    color: #ababab;

    &-active {
      color: #CD1212;
    }
  }
}

.decoration {
  color: #CD1212;
}

.list {
  list-style: none;
  padding: 0;

  &__item {
    visibility: hidden;
    display: inline;
    padding-right: 1rem;

    &-visible {
      visibility: visible;
    }
  }
}

.menu {
  list-style: none;
  display: flex;
  flex-direction: column;

  &__element {
    position: relative;
    line-height: 1.5;
    text-transform: uppercase;

    &::after {
      content: "";
      height: 1px;
      width: 0%;
      background-color: black;

      position: absolute;
      bottom: 0;
      left: 0;

      transition: width 0.5s ease;
    }

    &:hover {
        &::after {
          width: 100%;
        }
      }
  }
}

</style>
