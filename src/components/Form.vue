<template>
  <form class="form">
    <div class="container-pages">
      <h3>Vamos conversar!</h3>
      <input type="text" placeholder="Nome" />
      <div class="form-contact">
        <input type="email" placeholder="E-mail" />
        <input
          ttype="tel"
          pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"
          placeholder="Telefone"
        />
      </div>
      <textarea placeholder="Mensagem"> </textarea>
      <button type="button">Enviar</button>
    </div>
  </form>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.form {
  display: flex;
  justify-content: center;
  align-items: center;
  & > .container-pages {
    display: flex;
    flex-direction: column;
    padding: 24px;
    & > h3 {
      font-family: Poppins;
      font-size: 30px;
      line-height: 39px;
      letter-spacing: -0.015em;
      margin: 0 0 24px;
      @media (min-width: 700px) {
        font-size: 40px;
        line-height: 60px;
      }
    }
    & input {
      width: 100%;
      margin: 10px 0;
      padding: 8px;
      box-sizing: border-box;

      display: flex;
      align-items: center;
    }
    & > .form-contact {
      display: flex;
      flex-direction: column;
      @media (min-width: 700px) {
        flex-direction: row;
      }
      & input:first-child {
        @media (min-width: 700px) {
          margin-right: 10px;
        }
      }
    }
    & > textarea {
      width: 100%;
      margin: 10px 0;
      padding: 8px;
      box-sizing: border-box;
      height: 120px;
    }

    & > button {
      width: 100%;
      margin: 10px 0;
      background: #2e9af9;
      box-shadow: 0px 0px 4px #2e9af9;
      border-radius: 3px;
      border: none;
      padding: 14px;
      color: #fff;
      cursor: pointer;

      @media (min-width: 768px) {
        width: 15%;
        align-self: flex-end;
      }

      &:hover {
        background: #60aef3;
      }
    }
  }
}
</style>
