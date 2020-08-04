<template>
  <Layout>
    <section class="container-lab" id="lab">
      <div class="content">
        <h1>I3Tech</h1>
        <p>
          Somos um lab focado no desenvolvimento de novas tecnologias para
          todos!
        </p>
      </div>
    </section>

    <section class="container-about" id="sobre">
      <div class="container-pages">
        <div class="content">
          <div>
            <h3>Pesquisa e desenvolvimento</h3>
            <p>
              Grandes empresas, normalmente possuem seus próprios labs de
              inovação, mas entendemos que essa não é a realidade para a maioria
              das pequenas e médias empresas no Brasil.
            </p>
            <p>
              Pensando nisso,criamos nosso lab, focado na exploração de
              tecnologias emergentes para quem precisar.
            </p>
          </div>
        </div>
        <div class="content">
          <ul class="list">
            <li class="item">
              <div class="icon">
                <g-image src="~/assets/image/blockchain.svg" />
              </div>
              <div class="text">
                <h4>Blockchain</h4>
                <p>
                  Ledger compartilhado e imutavel para a gravação de transações,
                  rastreamento de ativos e auditoria transparente.
                </p>
              </div>
            </li>

            <li class="item">
              <div class="icon">
                <g-image src="~/assets/image/machine-learning.svg" />
              </div>
              <div class="text">
                <h4>Machine Learning</h4>
                <p>
                  Aplicação de algoritmos a grandes massas de dados para
                  extração de padrões e estatisticas e tomada de comportamentos
                  dos sitemas.
                </p>
              </div>
            </li>

            <li class="item">
              <div class="icon">
                <g-image src="~/assets/image/iot.svg" />
              </div>
              <div class="text">
                <h4>IoT</h4>
                <p>
                  LInternet das coisas, utilizada para realizar conexões
                  digitais entre objetos fisicos e a internet .
                </p>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </section>

    <section class="container">
      <div class="container-pages">
        <div class="text">
          <h3>
            Entendemos que inovação e tencnolgia não é exclusividade de grandes
            empresa!
          </h3>
          <p>
            Nossos produtos e serviços são focados para todos que tenham
            interesse em XXX.
          </p>
        </div>
        <g-image src="~/assets/image/graphic.png" />
      </div>
    </section>

    <section class="container-products" id="servicos">
      <div class="container-pages">
        <g-image src="~/assets/image/product.png" />
        <div class="text">
          <h3>Produtos e serviços</h3>
          <p>
            Com as tecnologias exploradas em nosso lab, nós entregamos serviços e
            produtos focados em inovação e tecnologia, como:
          </p>
          <ul>
            <li>Aplicativos</li>
            <li>Metodologias ageis</li>
            <li>Sistemas com a tecnologia blockchain</li>
          </ul>
        </div>
      </div>
    </section>
  </Layout>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container-lab {
  display: flex;
  align-items: center;
  width: 100%;
  height: 80vh;
  background: url("../assets/image/background.svg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  & > .content {
    width: 20%;
    margin: 16%;
    @media (max-width: 768px) {
      width: 42%;
      margin: 10%;
    }
    & > h1 {
      font-family: Poppins;
      font-weight: 500;
      font-size: 66px;
      line-height: 99px;
      letter-spacing: -0.015em;
      margin: 0;
      color: #18a0fb;
      @media (max-width: 768px) {
        font-size: 36px;
        line-height: 40px;
      }
    }
    & > p {
      font-size: 20px;
      line-height: 23px;
      letter-spacing: -0.015em;
      @media (max-width: 768px) {
        font-size: 14px;
        line-height: 18px;
        letter-spacing: -0.01em;
      }
    }
  }
}
.container-about {
  display: flex;
  align-items: center;
  justify-content: center;
  & > .container-pages {
    display: flex;
    padding: 24px;
    flex-direction: column;
    @media (min-width: 810px) {
      flex-direction: row;
      padding: 16px;
    }
    & > .content {
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      @media (min-width: 810px) {
        width: 50%;
      }
      & > div {
        & > h3 {
          font-family: Poppins;
          font-size: 28px;
          line-height: 113.5%;
          letter-spacing: -0.015em;
          color: #2e9af9;
          margin-top: 0;
          @media (min-width: 810px) {
            font-size: 40px;
          }
        }
      }
      & > p {
        font-size: 20px;
        line-height: 23px;
        letter-spacing: -0.015em;
      }

      & > .list {
        list-style: none;
        padding: 0;
        margin: 0;
        & > .item {
          display: flex;
          align-items: flex-start;
          justify-content: center;
          flex-direction: column;
          margin: 24px 0;
          @media (min-width: 810px) {
            height: 90px;
            align-items: center;
            justify-content: center;
            flex-direction: row;
          }
          & > .icon {
            width: 100%;
            height: 90px;
            align-items: center;
            justify-content: center;
            display: flex;
            background: #1a1a1a;
            border-radius: 9px;
            padding: 10px;
            height: 90px;
            margin-bottom: 20px;
            @media (min-width: 810px) {
              height: auto;
              margin: 0;
              width: 90px;
            }
          }
          & > .text {
            margin: 0;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            @media (min-width: 810px) {
              margin-left: 16px;
            }
            & > h4 {
              margin: 0;
              font-family: Poppins;
              font-weight: bold;
              font-size: 20px;
              line-height: 36px;
              letter-spacing: -0.015em;
              color: #2e9af9;
            }

            & > p {
              margin: 0;
              font-size: 15px;
              line-height: 18px;
              letter-spacing: -0.015em;
            }
          }
        }
      }
    }
        & > .content:first-child {
        @media (min-width: 810px) {
          margin-right: 60px;
        }
      }
  }
}

.container {
  background: #2e9af9;
  display: flex;
  justify-content: center;
  align-items: center;
  & > .container-pages {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 24px;
    flex-direction: column-reverse;
    @media (min-width: 700px) {
      flex-direction: row;
    }
    & > .text {
      @media (min-width: 700px) {
        margin-right: 32px;
      }
      & > h3 {
        font-family: Poppins;
        font-size: 28px;
        line-height: 38px;
        letter-spacing: -0.015em;
        font-weight: 100;
        @media (min-width: 700px) {
          width: 85%;
          font-size: 40px;
          line-height: 60px;
        }
      }
    }
    & > img {
      width: 270px;
      @media (min-width: 700px) {
        width: 25%;
      }
    }
  }
}
.container-products {
  display: flex;
  justify-content: center;
  align-items: center;
  & > .container-pages {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 24px;
    flex-direction: column;
    @media (min-width: 700px) {
      flex-direction: row;
    }

    & > img {
      width: 300px;
      @media (min-width: 700px) {
        width: auto;
      }
    }
    & > .text {
      width: 100%;
      @media (min-width: 700px) {
        width: 45%;
      }
      & > h3 {
        font-family: Poppins;
        font-size: 28px;
        line-height: 30px;
        letter-spacing: -0.015em;
        color: #2e9af9;

        @media (min-width: 700px) {
          font-size: 40px;
          line-height: 60px;
        }
      }
    }
  }
}
</style>
