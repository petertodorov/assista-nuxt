<template>
  <nav class="c-main-mobile-nav">
    <button class="c-main-mobile-nav__menu" @click="toggleMobileMenu()">
      <font-awesome-icon
        class="c-main-mobile-nav__menu__icon"
        :icon="['fas', 'bars']"
      />
    </button>
    <ul v-if="showMobileMenu" class="c-main-mobile-nav__list">
      <li class="c-main-mobile-nav__list-item">
        <a href="#" class="c-main-mobile-nav__list-item__link">How it works</a>
      </li>
      <li class="c-main-mobile-nav__list-item">
        <a href="#" class="c-main-mobile-nav__list-item__link">Tour features</a>
      </li>
      <li class="c-main-mobile-nav__list-item">
        <a href="#" class="c-main-mobile-nav__list-item__link">Pricing</a>
      </li>
      <li class="c-main-mobile-nav__list-item">
        <a href="#" class="c-main-mobile-nav__list-item__link">FAQs</a>
      </li>
      <li class="c-main-mobile-nav__list-item">
        <a href="#" class="c-main-mobile-nav__list-item__link">My time</a>
      </li>
    </ul>
  </nav>
</template>
<script>
export default {
  name: 'MainNavigation',
  data() {
    return {
      showMobileMenu: false,
    }
  },
  methods: {
    toggleMobileMenu() {
      this.showMobileMenu = !this.showMobileMenu
    },
  },
}
</script>
