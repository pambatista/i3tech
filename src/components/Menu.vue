<template>
  <nav class="nav">
    <g-image src="~/assets/image/logo.svg" alt="i3tech logo" class="logo" />
    <div class="line" />
    <div class="nav-menu">
      <g-link class="nav__link" to="/">lab</g-link>
      <g-link class="nav__link" to="/about/">Serviços</g-link>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
    .nav {
    display: flex;
    align-items: center;
      & > .logo {
        @media (max-width: 768px) {
          width: 70px;
        }
      }
      & > .line {
        width: 100%;
        height: 2px;
        background: #2E9AF9;
        box-shadow: 0px 0px 3px #2E9AF9;
      }
      & > .nav-menu {
        & > .nav__link {
          display: none;
          margin: 0 16px;
          font-size: 16px;
          line-height: 18px;
          letter-spacing: -0.015em;
          text-decoration: none;
          color: #2E9AF9;
          text-shadow: 0px 0px 3px #2E9AF9;
          @media (min-width: 768px) {
            display: inline;
            margin: 0 24px;
            font-size: 20px;
            line-height: 23px;
          }
        }
      }
  }
</style>
