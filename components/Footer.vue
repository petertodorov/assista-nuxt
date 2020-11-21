<template>
  <footer class="c-main-footer">
    <div class="o-content-page-wrapper">
      <section class="footer__logo-and-copyright">
        <a
          href="https://camplight.net/"
          class="footer__logo-and-copyright__logo-container"
        >
          <img src="./../static/cl_logo.png" alt="Campligh logo" />
        </a>
        <p class="footer__logo-and-copyright__copyright">
          © Copyright 2020. All rights reserved.
        </p>
      </section>
      <section class="footer__external-links">
        <a
          class="footer__external-links__link"
          href="mailto:assista@camplight.net"
        >
          <font-awesome-icon :icon="['fas', 'envelope']" />
        </a>
        <a
          class="footer__external-links__link"
          href="https://www.facebook.com/camplight/"
        >
          <font-awesome-icon :icon="['fab', 'facebook-square']" />
        </a>
      </section>
      <section class="footer__privacy">
        <p class="footer__privacy__text">
          We are not affiliated, associated, authorized, endorsed by or in any
          way officially connected to Trello, Inc.
        </p>
        <a href="#" class="footer__privacy__link"
          >Privacy terms and conditions</a
        >
      </section>
    </div>
  </footer>
</template>
