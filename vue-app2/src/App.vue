<template>
  <div id="nav">

    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a class="navbar-item">
          <img class="logo" src="../src/assets/logop.png" />
          <h2>ORTAONLINE</h2>
        </a>  


        <a
          role="button"
          class="navbar-burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="navMenu"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div
        id="navMenu"
        class="navbar-menu"
        v-bind:class="{ 'is-active': isActive }"
      >
        <div class="navbar-start">
          <a class="navbar-item">
            <router-link to="/">Home</router-link>
          </a>

          <a class="navbar-item">
            <router-link to="/about">About</router-link>
          </a>
        </div>

        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <a class="button">
                <strong>Adquira Já</strong>
              </a>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <router-view/>
    
    <div class="footer">
      <br />
      <p>
        <img src="../src/assets/logoescrita.png" />
        || Copyright © Portãonline 2021 ||
        <a href="https://github.com/carloshmedeiros">
        <img id="git" src="../src/assets/gitlogo.png"/>
        </a>
      </p>
    </div>
  </div>
</template>

<script>

export default {
  name: "app",
};

document.addEventListener("DOMContentLoaded", () => {
  // Get all "navbar-burger" elements
  const $navbarBurgers = Array.prototype.slice.call(
    document.querySelectorAll(".navbar-burger"),
    0
  );

  // Check if there are any navbar burgers
  if ($navbarBurgers.length > 0) {
    // Add a click event on each of them
    $navbarBurgers.forEach((el) => {
      el.addEventListener("click", () => {
        // Get the target from the "data-target" attribute
        const target = el.dataset.target;
        const $target = document.getElementById(target);

        // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu"
        el.classList.toggle("is-active");
        $target.classList.toggle("is-active");
      });
    });
  }
});
</script>

<style lang="scss">
@import "./node_modules/bulma/bulma.sass";
@import "mq";
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
  background: url(../src/assets/banner1.png);
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

#git {
  width: 30px;
  margin-bottom: -10px;
  margin-left: 2px;
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
