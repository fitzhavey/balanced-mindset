<template>
  <div class="bmPage">
    <h1>Balanced Mindset</h1>
    <div class="bmPage__quote">
      <p class="bmPage__quote__text">
        If you feel like a mess, remember that a star is just a big pile of space
        trash that pulled itself together and will shine for billions of years. Be
        messy like space trash and shine like the star you are~
      </p>
      <div class="bmPage__quote__overlay">
        <img class="bmPage__quote__image" src="~/assets/sun.gif"/>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LandingPage',
}
</script>

<style lang="scss">
.bmPage {
  margin: 1rem;

  &__quote {
    position: relative;

    &__text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: black;
      font-weight: bold;
      width: 90%;
      z-index: 2;
    }

    &__overlay {
      width: 100%;
      height: 100%;
      background-color: grey;
      opacity: 30%;
      z-index: 1;
    }

    &__image {
      width: 100%;
      z-index: 0;
      border-radius: 1rem;
    }

  }
}
</style>
