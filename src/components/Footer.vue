<template>
  <footer class="footer">
    <g-image src="~/assets/image/logo.svg" alt="i3tech logo" class="logo" />
    <div class="line" />
    <div class="social-content">
      <a href="#" target="_blank" class="social-icon">
        <g-image src="~/assets/image/icon/instagram.svg"/>
      </a>

      <a href="#" target="_blank" class="social-icon">
        <g-image src="~/assets/image/icon/linkedin.svg"/>
      </a>

      <a  href="#" target="_blank" class="social-icon">
        <g-image src="~/assets/image/icon/facebook.svg"/>
      </a>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .footer {
    display: flex;
    align-items: center;
    padding: 16px;
    @media (min-width: 768px) {
      padding: 32px;
    }
      & > .logo {
        width: 40px;
        @media (min-width: 700px) {
          width: 90px;
        }
      }
      & > .line {
        width: 100%;
        height: 1px;
        background: #2E9AF9;
        box-shadow: 0px 0px 3px #2E9AF9;
        @media (min-width: 700px) {
          height: 2px;
        }
      }

      & > .social-content {
        display: flex;
        & > .social-icon {
          display: flex;
          align-items: center;
          justify-content: center;
          margin-left: 5px;
          background: #1A1A1A;
          border: 2px solid #2E9AF9;
          box-sizing: border-box;
          box-shadow: inset 0px 4px 4px rgba(0, 0, 0, 0.25);
          border-radius: 9px;
          padding: 5px;
          @media (min-width: 700px) {
            padding: 10px 12px;
            margin-left: 16px;
            border: 3px solid #2E9AF9;
          }
          & > img {
            width: 20px;
            @media (min-width: 700px) {
              width: 28px;
            }
          }
          &:hover {
            background: #2E9AF9;
          }
        }
      }
  }

</style>
