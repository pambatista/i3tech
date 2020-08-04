<template>
  <div class="layout">
    <header class="header">
      <Menu />
    </header>
    <slot/>
    <Form />
    <Footer />
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
import Footer from '~/components/Footer.vue'
import Form from '~/components/Form.vue'

export default {
  components: {
    Menu,
    Footer,
    Form
  }
}
</script>

<style lang="scss">
body {
  margin:0;
  padding:0;
  line-height: 1.5;
  background: #040404;
  color: #fff;
}

body,
input,
button,
textarea {
  font-family: 'Roboto', sans-serif;
  font-size: 14px;
  line-height: 21px;
  letter-spacing: -0.015em;
  outline: none;

  @media (min-width: 700px) {
    font-size: 18px;
    line-height: 21px;
  }

  &::placeholder {
    color: #1f1f1f;
  }
}

.container-pages {
  width: 90vw;
  max-width: 1200px;
}
* {
  box-sizing: border-box;
}
</style>
