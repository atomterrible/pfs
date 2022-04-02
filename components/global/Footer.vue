<template>
  <footer>
    <div class="connect">
      <nuxt-link to="/"><img class="logo" src="~/static/img/logo.png" alt="Pro Film Sound Logo" /></nuxt-link>
      <p>
        Call or text for questions.<br />
        <a href="tel:19403674447">940-367-4447</a>
      </p>
      <p class="text-xs">Copyright © 2022 Adam Terrell</p>
    </div>
    <div class="menu">
      <h5>Navigate</h5>
      <nav>
        <ul>
          <li><nuxt-link to="/work">Work</nuxt-link></li>
          <li><nuxt-link to="/services">Services</nuxt-link></li>
          <li><nuxt-link to="/about">About</nuxt-link></li>
          <li><nuxt-link to="/contact">Contact</nuxt-link></li>
        </ul>
      </nav>
    </div>
    <div class="policies">
      <h5>Policies</h5>
      <nav>
        <ul>
          <li><nuxt-link to="privacy-policy">Privacy Policy</nuxt-link></li>
          <li><nuxt-link to="terms-of-service">Terms of Service</nuxt-link></li>
        </ul>
      </nav>
    </div>
    <div class="connect">
      <h5>Connect</h5>
      <nav>
        <ul>
          <li><a href="https://instagram.com/adamcterrell" target="_blank">Instagram</a></li>
          <li><a href="https://www.youtube.com/user/atomterrible" target="_blank">YouTube</a></li>
        </ul>
      </nav>
    </div>
  </footer>
</template>

<style lang="postcss" scoped>
footer {
  @apply flex w-full bg-primary-800 mx-auto place-content-center place-items-center flex-col p-6 text-center lg:flex-row lg:justify-items-stretch lg:justify-between lg:items-start lg:content-start lg:text-left lg:p-14;

  div {
    @apply p-4 mx-auto lg:m-0 lg:p-0;
  }

  h5 {
    @apply mb-2;
  }

  .logo {
    @apply max-w-[140px] mb-6 m-auto lg:m-0;
  }

  li {
    @apply leading-10;
  }
}
</style>

<script>
export default {
  name: 'Footer',
}
</script>