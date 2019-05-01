<template>
  <section class="section-contact" id="contact">
    <div class="section-contact__content">
      <h1 class="section-contact__header">Lets talk! :)</h1>
      <div class="section-contact__contact-info"> 
        <div class="section-contact__contact-info__email">
          <p class="section-contact__contact-info__label">Email:</p>
          <p class="section-contact__contact-info__detail">aruffincs@gmail.com</p>
        </div>
        <div class="section-contact__contact-info__phone">
          <p class="section-contact__contact-info__label">Phone #:</p>
          <p class="section-contact__contact-info__detail">757-450-3114</p>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'section-contact'
}
</script>
<style lang="scss">
@import '../assets/global-styles.scss';

.section-contact {
  height: $section-height;
  display: flex;
  justify-content: center;
  vertical-align: middle;

  &__content {
    align-self: center;
  }

  &__header {
    font-size: $section-header-font-size-mobile;
    border-bottom: $color-light-green solid 4px;
    margin: 0 auto;
    display: inline-block;

    @include for-desktop {
      font-size: $section-header-font-size-desktop;
    }
  }

  &__contact-info {
    &__label {
      font-size: 1.2rem;
    }

    &__detail {
      font-size: 1.8rem;
      color: $color-light-green;
    }

    &__email {
      padding-top: 3rem;
      margin: 4rem auto;
    }
  }
}
</style>
