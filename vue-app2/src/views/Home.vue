<template>
  <div class="home">
  <section class="hero is-danger is-fullheight">
      <div class="hero2">
        <div class="hero-body">
          <p class="title">
            O FUTURO <br />
            DA SUA CASA <br />NA PALMA <br />
            DA SUA MÃO
          </p>
          <img src="@/assets/logop2.png" />
          <p class="aa"></p>
        </div>
      </div>
    </section>

    <div class="division"></div>

    <h1 class="textosection">O FUTURO CHEGOU</h1>
    <section class="hero is-large is-info">
      <div class="hero1">
        <div class="about__bg">
          <div class="section__inner">
            <div class="about__mission">
              <img src="@/assets/mission.png" />
              <h3>MISSÃO</h3>
              <p>
                Desenvolver soluções tecnológicas que proporcionem bem-estar às
                pessoas.
              </p>
            </div>
            <div class="about__vision">
              <img src="@/assets/vision.png" />
              <h3>VISÃO</h3>
              <p>Trazer conforto e praticidade para as pessoas.</p>
            </div>
            <div class="about__values">
              <img src="@/assets/values.png" />
              <h3>VALORES</h3>
              <p>Inovação, qualidade, minimalismo e tecnologia.</p>
            </div>
          </div>
        </div>
      </div>
    </section>


    <h1 class="textosection2">CONTROLE SUA CASA</h1>
    <section class="herodois">
      <div class="hero-body">
        <div class="about__bg">
          <div class="section__inner">
            <div class="controle_section">
              <img class="check" src="@/assets/check.png" />
              <h3>CONTROLE DE ONDE QUISER</h3>
              <p>
                O aplicativo Portãonline permite o acionamento do mecanismo
                desejado de qualquer lugar graças a tecnologia de wi-fi
                integrado.
              </p>
            </div>
            <div class="facil_section">
              <img class="check" src="@/assets/check.png" />
              <h3>FACIL E PRÁTICO</h3>
              <p>
                Acessibilidade é um fator essencial, com o Portãonline você não
                precisa perder tempo procurando o controle de seu portão, ele
                está no seu celular e pode ser acessado com um simples clique.
              </p>
            </div>
            <div class="seguranca_section">
              <img class="check" src="@/assets/check.png" />
              <h3>SEGURANÇA EM 1° LUGAR</h3>
              <p>
                Nosso sistema conta com uma tela de login, assegurando proteção
                e conforto para o usuário.
              </p>
            </div>
            <img class="phone" src="@/assets/cel2.png" />
          </div>
        </div> 
      </div>
    </section>


    <h1 class="textosection3">GARANTA JÁ O SEU!</h1>
    <section class="herotres">
      <div class="hero-body">
        <div class="field">
          <label class="label">Nome</label>
          <div class="control">
            <input class="input" type="text" placeholder="Text input" />
          </div>
        </div>

        <div class="field">
          <label class="label">Email</label>
          <div class="control has-icons-left has-icons-right">
            <input
              class="input is-danger"
              type="email"
              placeholder="Email input"
              value="hello@"
            />
            <span class="icon is-small is-left">
              <i class="fas fa-envelope"></i>
            </span>
            <span class="icon is-small is-right">
              <i class="fas fa-exclamation-triangle"></i>
            </span>
          </div>
          <p class="help is-danger">Email inválido</p>
        </div>

        <div class="field">
          <label class="label">Mensagem</label>
          <div class="control">
            <textarea class="textarea" placeholder="Textarea"></textarea>
          </div>
        </div>

        <div class="field is-grouped">
          <div class="control">
            <div class="buttons">
              <a class="button submit">
                <strong>Enviar</strong>
              </a>
            </div>
          </div>
          <div class="control">
            <button class="button is-link is-light">Cancel</button>
          </div>
        </div>
      </div>
    </section>  
    </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
};
</script>

<style lang="scss">
@import "./node_modules/bulma/bulma.sass";
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Roboto+Condensed&family=Zen+Maru+Gothic&display=swap");

/* MENU */

.navbar {
  background: linear-gradient(140deg, #292929 55%, #9db288 0);
  position: fixed;
  width: 100%;
}

.navbar h2 {
  color: #fff;
}

.navbar a {
  color: #838282;
}

.button {
  background-color: #292929;
}

a.button {
  color: #fff;
  &:hover {
    color: #9db288;
  }
}

a.navbar-burger {
  color: rgb(0, 0, 0);
}

a.r-item {
  color: #c1c1c1;
  + mobile {
    color: gray;
    &:hover {
      background-color: #f1f1f1;
    }
  }
}

.divisionnav {
  height: 10px;
  background: #a50808;
  margin-left: auto;
  margin-right: auto;
}

.division {
  height: 5px;
  width: 200px;
  background: #292929;
  margin: 20px 0px 20px 0px;
  margin-left: auto;
  margin-right: auto;
}

/* BANNER */

.hero2 {
  background: url(../assets/banner1.png);
  background-size: cover;
  .hero-body {
    width: 2600px;
    background: linear-gradient(90deg, #292929 20%, #ffffff00 0);
    max-width: 2600px;
    img {
      width: 110px;
      margin: 600px 0px 0px -270px;
    }
  }
}

.title {
  font-size: 110px;
  font-family: "Bebas Neue", cursive;
}

.aa {
  margin-bottom: 850px;
}

/* MISSION VISION VALUES */

.textosection {
  margin-top: 70px;
  font-family: "Bebas Neue", cursive;
  font-size: 60px;
  text-align: center;
}

.about__mission,
.about__values,
.about__vision {
  float: left;
  text-align: center;
  padding: 0 40px;
  color: black;
  width: 33%;
  img {
    margin-bottom: -10px;
    width: 100px;
  }
}

.hero1 {
  background-color: white;
  height: 300px;
  .container,
  .pageHeader__inner,
  .section__inner {
    margin-left: auto;
    margin-right: auto;
    padding-left: 0.9375rem;
    padding-right: 0.9375rem;
    max-width: 75rem;
  }
  h3 {
    font-family: "Roboto Condensed", sans-serif;
    font-weight: bold;
    font-size: 25px;
  }
  p {
    font-size: 18px;
    font-family: "Zen Maru Gothic", sans-serif;
  }
}

/* section */

.division2 {
  height: 5px;
  width: 200px;
  background: #942525;
  margin: 20px 0px -10px 0px;
  margin-left: auto;
  margin-right: auto;
}

.textosection2 {
  padding-top: 70px;
  font-family: "Bebas Neue", cursive;
  font-size: 60px;
  text-align: center;
  background-color: #292929;
  color: rgb(161, 161, 161);
}

.herodois {
  .container,
  .pageHeader__inner,
  .section__inner {
    margin-left: 150px;
    max-width: 150rem;
  }
  .hero-body {
    background-color: #292929;
    .check {
      width: 25px;
      float: left;
      margin-left: -50px;
      margin-top: 10px;
    }
    .phone {
      width: 800px;
      float: right;
      margin: -600px 150px 0px 0px;
    }
    h3 {
      margin-top: 60px;
      font-family: "Roboto Condensed", sans-serif;
      font-weight: bold;
      font-size: 35px;
      color: #fff;
    }
    p {
      font-size: 25px;
      font-family: "Zen Maru Gothic", sans-serif;
      color: rgb(161, 161, 161);
    }
  }
}

.controle_section,
.facil_section,
.seguranca_section {
  padding: 0px 40px;
  color: black;
  width: 33%;
  img {
    margin-bottom: -10px;
    width: 100px;
  }
}

/* RODAPE */

.footer {
  left: 0;
  bottom: 0;
  width: 100%;
  background-color: #292929;
  color: rgb(161, 161, 161);
  text-align: center;
  padding-top: 0px;
  padding-bottom: 25px;
  padding-left: 10px;
  padding-right: 10px;
  img {
    width: 200px;
    margin-bottom: -25px;
    margin-right: -15px;
  }
  i:hover {
    color: #aec6cf;
    transition: 0.4s;
    cursor: pointer;
  }
}

#icon {
  margin-left: 5px;
}

.textosection3 {
  padding-top: 70px;
  background-color: #9db288;
  font-family: "Bebas Neue", cursive;
  font-size: 60px;
  text-align: center;
}

.herotres {
  .hero-body {
    background-color: #9db288;
  }
}
</style>

