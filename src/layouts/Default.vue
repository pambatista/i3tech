<template>
  <div class="layout">
    <header class="header">
      <Menu />
    </header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
import Menu from '~/components/Menu.vue'
export default {
  components: {
    Menu
  }
}
</script>

<style lang="scss">
body {
  font-family: 'Roboto', sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
  background: #040404;
  color: #fff;
}
.layout {
  padding: 32px;
}
</style>
