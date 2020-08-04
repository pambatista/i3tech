<template>
<div>
  <nav class="nav">
    <g-image src="~/assets/image/logo.svg" alt="i3tech logo" class="logo" />
    <div class="line" />
    <g-image src="~/assets/image/icon/menu-aberto.svg" alt="i3tech logo" class="menu" @click="openMenu"/>
    <div class="nav-menu">
      <g-link class="nav__link" to="/#sobre">lab</g-link>
      <g-link class="nav__link" to="/#servicos">Serviços</g-link>
    </div>
  </nav>
  <transition name="fade">
    <div v-if="hasMenu" :class="['menu-drop' , {hasMenu: 'menu-open'}]">
      <g-link  to="/#sobre">lab</g-link>
      <g-link  to="/#servicos">Serviços</g-link>
    </div>
  </transition>
</div>

</template>

<script>
export default {
  data() {
    return {
      hasMenu: false,
    }
  },
  methods: {
    openMenu() {
      console.log('clicou')
      this.hasMenu = !this.hasMenu
    }
  }
};
</script>

<style lang="scss" scoped>
    .nav {
    padding: 16px 16px 0;
    @media (min-width: 768px) {
      padding: 32px 32px 0;
    }
    display: flex;
    align-items: center;

      & > .logo {
        width: 40px;
        @media (min-width: 700px) {
          width: 90px;
        }
      }
      & > .menu {
        width: 30px;
        margin-left: 10px;
        @media (min-width: 700px) {
          display: none;
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
          &:hover {
            color: #fff;
          }
        }
      }
  }
  .menu-drop {
    position: absolute;
    width: 70%;
    right: 0;
    display: flex;
    flex-direction: column;
    padding: 20px;
    background: #080808;
    transition: max-height 1s;
    border-radius: 10px;
    & > a {
      text-align: end;
      font-size: 16px;
      line-height: 18px;
      letter-spacing: -0.015em;
      text-decoration: none;
      color: #2E9AF9;
      text-shadow: 0px 0px 3px #2E9AF9;
      padding: 10px 0;
    }
  }
.fade-enter-active, .fade-leave-active {
  transition: opacity .3s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
</style>
