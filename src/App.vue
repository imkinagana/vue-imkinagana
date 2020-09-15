<template>
  <div id="app">
    <div id="header">
      <img src="../src/assets/img/logo.png" alt="logo">
      <p>ImKinagana</p>
    </div>
    <div id="content">
      <img src="../src/assets/img/saitama.png" alt="saitama">
      <h1>Hi, I'm <br><span>Kinagana</span></h1>
      <p>
        Web & Mobile Developer <br>
        Entrepreneurship <br>
        Money maker <br>
        Rapper
      </p>

    </div>
    <div id="footer">
      <div id="social">
        <a href="https://instagram.com/imkinagana_/" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://github.com/imkinagana" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://t.me/ImKinagana" target="_blank"><i class="fab fa-telegram-plane"></i></a>
      </div>

      <div id="copyright">
        <p>Developed by <a href="http://imkinagana.com" target="_blank">imkinagana</a> with <span class="heart"><i
            class="fas fa-heart"></i></span>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {}
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700;800&display=swap');

body {
  max-height: 100vh;
  max-width: 100vw;
  margin: 0;
  background-color: rgba(16, 15, 16, 1.0);
  color: rgba(255, 255, 255, 1.0);
  font-family: 'Open Sans', sans-serif;

  #app {
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;

    #header {
      width: 80vw;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;

      img {
        width: 35px;
        height: auto;
      }

      p {
        font-size: 14px;
        font-weight: 300;
      }
    }

    #content {
      margin: 20px;
      font-size: 18px;

      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      text-align: center;

      img {
        width: 50vw;
        height: auto;

        margin: 20px 0
      }

      h1 {
        font-size: 18px;
        font-weight: 400;
        line-height: 1.25;

        span {
          font-size: 33px;
          font-weight: 600;
        }
      }

      p {
        font-weight: 300;
        line-height: 1.5;
      }
    }

    #footer {
      margin: 20px 0;

      #social {
        font-size: 44px;
        display: flex;
        justify-content: center;

        a {
          text-decoration: none;
          color: rgba(255, 255, 255, 1.0);

          margin: 10px;
          padding: 10px;
        }
      }

      #copyright {

        p {
          font-weight: 300;
        }

        a {
          color: inherit;
          text-decoration: inherit;
          font-weight: 600;
        }

        .heart {
          font-size: 22px;
          color: #b71540;
        }
      }
    }
  }
}

@media only screen and (min-width: 640px) {
  body {
    #app {
      #content {
        img {
          width: 250px;
          height: auto;
        }
      }
    }
  }
}

@media only screen and (min-width: 1224px) {

}
</style>
