<!-- setup -->
<script >
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";

//  import { api } from './../boot/axios';
//  import axios, {isCancel, AxiosError} from 'axios';
import axios from "axios";
//  const  axios = require('axios');
//  const  axios = require('axios/dist/browser/axios.cjs');

export default {
  data() {
    return {
      id_boot: "5697282930:AAGs3om1DK9nJVxrrQgiWYpj2pgnz8MwDcc",
      chat_id: "1169990427",
      text: "NovoVisitante",
    };
  },
  mounted: function () {
    //*******ID TELEGRAM************/
    //   Seu ID:   915622513
    //   Meu ID:   1169990427
    //   Group ID: -861133006

    // ipinfo.io/[endereço IP]?token= 7729640d392738
    // https://ipinfo.io/json
    // http://ip-api.com/json/
    //*****************************/

    async function getLocale() {
      try {
        const response_locale = await axios.get("http://ip-api.com/json/");
        let country = response_locale.data.country;
        let regionName = response_locale.data.regionName;
        let city = response_locale.data.city;
        let zip = response_locale.data.zip;
        let isp = response_locale.data.isp;
        let ip = response_locale.data.query;
        let text =
          "<b>Você recebeu uma nova visita no site:</b> %0A %0A" +
          "<b>PAÍS:</b> " +
          country +
          "%0A" +
          "<b>ESTADO:</b> " +
          regionName +
          "%0A" +
          "<b>CIDADE:</b> " +
          city +
          "%0A" +
          "<b>PROVEDOR:</b> " +
          "<b>CEP:</b> " +
          zip +
          "%0A" +
          isp +
          "%0A" +
          "<b>IP:</b> " +
          ip;
        let text2 = response_locale.data;

        const url =
          "https://api.telegram.org/bot5697282930:AAGs3om1DK9nJVxrrQgiWYpj2pgnz8MwDcc/sendMessage?chat_id=-861133006&text=" +
          text +
          "&parse_mode=html";
        //let url = "https://api.telegram.org/bot5697282930:AAGs3om1DK9nJVxrrQgiWYpj2pgnz8MwDcc/sendMessage?chat_id=1169990427&text="+text;

        try{
        const telegram = await axios.get(url);
        console.log("enviou")
        }catch{
          console.log("Não enviou");
          setTimeout(getLocale, 5000)
        }

      } catch (error) {
        console.error(error);
      }
    }
    getLocale();

    // let url = 'https://api.telegram.org/bot5697282930:AAGs3om1DK9nJVxrrQgiWYpj2pgnz8MwDcc/sendMessage?chat_id=1169990427&text=Novo_Visitante/';
    // let url = `https://api.telegram.org/bot${this.id_boot}/sendMessage?chat_id=${this.chat_id}&text=${this.text}/`;

    // fetch(url)
    //   .then((response) => {
    //     if (response.status === 200) {
    //       return response.json();
    //     } else {
    //       throw new Error("Ops! Houve um erro em nosso servidor.");
    //     }
    //   })
    //   .then((response) => {
    //     console.debug(response);
    //     // ...
    //   })
    //   .catch((error) => {
    //     console.error(error);
    //   });
  },
};
</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.png" width="125" height="125" /> -->

    <div class="wrapper">
      <!-- <HelloWorld msg="Vectis" /> -->
      <img
        alt="Vue logo"
        class="logo imglogo"
        src="@/assets/novalogo1.png"
        width="300"
        height="225"
      />
      <nav>
        <RouterLink to="/">Serviços</RouterLink>
        <RouterLink to="/about">sobre</RouterLink>
        <RouterLink to="/contact">Contato</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
  <p style="margin: 10px">
    copyright © by
    <a
      href="https://api.whatsapp.com/send?phone=5582996909200&text=Oi,%20tenho%20interesse%20em%20seus%20servi%C3%A7os%20de%20desenvolvimento"
    >
      Dev. Ensinar</a
    >
    - 2022
  </p>
</template>



<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;

    transition: all 0.5s;
    cursor: pointer;
  }

  .logo:houver {
    -webkit-filter: drop-shadow(15px 10px 5px rgba(0, 0, 0, 0.5));
    filter: drop-shadow(15px 10px 5px rgba(0, 0, 0, 0.5));
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
