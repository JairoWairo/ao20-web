<template>
  <main class="-mt-32 -z-1">
    <header class="relative overflow-hidden" style="background: initial">
      <div class="container h-full flex justify-center items-center sticky z-20 pt-32 py-16 sm:pt-24 md:pt-32 lg:pt-40 xl:pt-48">
        <div class="flex flex-col items-center">
          <img src="@/assets/img/argentum20_logo.png" alt="Argentum 20 Logo" class="w-96 mb-3 xl:mb-6 no-select" />
          <h1 class="text-xl sm:text-3xl text-center leading-tight text-white mb-12 normal-case">
            Aventurate en las tierras de Argentum 20<br class="hidden lg:block" />
            y escribí tu propio camino
          </h1>
          <a href="/#juga-gratis" class="btn btn-cta">Jugá gratis</a>
        </div>
      </div>

      <div class="bg-black opacity-50 absolute top-0 left-0 w-full h-full object-cover z-10"></div>

      <img :src="homePage.data.banner_image.url" alt="" class="w-full h-full absolute top-0 left-0 object-cover bg-transparent" />

    </header>

    <div class="container-flex h-3 bg-divider-texture bg-repeat-x bg-center"></div>
    <br>
    <br>
    <section id="apoyanos" class="container max-w-screen-lg mx-auto">
      <h3 class="section-title mb-10 text-center">¡Apoyanos!</h3>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-10 md:gap-16 md:text-lg">
        <article class="flex flex-col gap-y-6">
          <h3 class="flex items-center gap-x-4 font-sans font-semibold text-xl md:text-2xl tracking-widest">
            <img src="@/assets/img/patreon.png" alt="Patreon" />
            Patreon
          </h3>
          <p>
            Convertite en un Patron para obtener beneficios exclusivos in-game y acceso a canales privados de Discord.
            <a class="section-title" href="https://www.patreon.com/posts/guia-beneficios-63817246" target="_blank">Ver beneficios patreons</a>
          </p>
          <div class="hidden md:flex flex-grow"></div>
          <a
            href="https://patreon.com/nolandstudios"
            target="_blank"
            rel="noopener"
            class="btn btn-silver self-start text-base"
            >Convertite en Patron
          </a>
        </article>

        <article class="flex flex-col gap-y-6">
          <h3 class="flex items-center gap-x-4 font-sans font-semibold text-xl md:text-2xl tracking-widest">
            <img src="@/assets/img/cafecito.png" alt="icono de cafecito" />
            Cafecito
          </h3>
          <div class="flex-grow">
            <p class="mb-3">Ayudanos con un Cafecito (psst, ¡lo creó Midraks, un jugador de AO!).</p>
            <p>¡Podés pagar con Mercado Pago y todos los medios que ofrece!</p>
          </div>
          <a
            href="https://cafecito.app/nolandstudios"
            target="_blank"
            rel="noopener"
            class="btn btn-silver self-start text-base"
            >Donar en Cafecito</a
          >
        </article>

        <!-- <img src="https://i.ibb.co/Tg22HDn/image.png" alt="Beneficios" /> -->


      </div>
    </section>

    <div class="section-divider my-16"></div>

    <!-- <section id="discord" class="container max-w-screen-lg mx-auto">
      <widgetbot
        server="761213868352471040"
        channel="761286044229959701"
        width="800"
        height="600"
      ></widgetbot>
      <script src="https://cdn.jsdelivr.net/npm/@widgetbot/html-embed"></script>
    </section> -->

    <section class="container max-w-screen-lg mx-auto">
        <h2 class="section-title text-center mb-4 md:mb-10">Novedades</h2>
      <div class="pb-3 md:pb-6 lg:pb-12">
        <News-Bar />
      </div>
    </section>

    <div class="container-flex h-3 bg-divider-texture bg-repeat-x bg-center"></div>

    <section class="bg-gray-1000">

      <div class="py-3 md:py-6 lg:py-12">
        <div class="container flex justify-center items-center gap-x-6 md:gap-x-10 lg:gap-x-20">
          <h3 class="font-sans font-normal sm:text-lg md:text-2xl lg:text-4xl">Seguinos</h3>
          <div class="flex items-center gap-x-2 lg:gap-x-12">
            <a
              href="https://discord.gg/e3juVbF"
              target="_blank"
              rel="noopener"
              class="transition-colors duration-150 ease-out text-[#6E85D3]"
            >
              <!-- <i class="fab fa-discord fa-2x"></i> -->
              <img src="@/assets/img/ico-discord.png" alt="icono discord" class="w-8 lg:w-20" />
            </a>
            <a
              href="https://github.com/ao-org"
              target="_blank"
              rel="noopener"
              class="transition-colors duration-150 ease-out text-[#6E85D3]"
            >
              <!-- <i class="fab fa-discord fa-2x"></i> -->
              <img src="@/assets/img/ico-github.png" alt="icono github" class="w-8 lg:w-20" />
            </a>
            <a
              href="https://www.youtube.com/c/PabloMarquez-aka-morgolock"
              target="_blank"
              rel="noopener"
              class="transition-colors duration-150 ease-out text-[#F70000]"
            >
              <!-- <i class="fab fa-youtube fa-2x"></i> -->
              <img src="@/assets/img/ico-youtube.png" alt="icono youtube" class="w-8 lg:w-20" />
            </a>
            <a
              href="https://www.facebook.com/ao20oficial"
              target="_blank"
              rel="noopener"
              class="transition-colors duration-150 ease-out text-[#1873EB]"
            >
              <!-- <i class="fab fa-facebook fa-2x"></i> -->
              <img src="@/assets/img/ico-facebook.png" alt="icono youtube" class="w-8 lg:w-20" />
            </a>
            <a
              href="https://instagram.com/ao20oficial"
              target="_blank"
              rel="noopener"
              class="transition-colors duration-150 ease-out text-[#DC3A60]"
            >
              <!-- <i class="fab fa-instagram fa-2x"></i> -->
              <img src="@/assets/img/ico-instagram.png" alt="icono instagram" class="w-8 lg:w-20" />
            </a>
            <a
              href="https://twitter.com/ao20oficial"
              target="_blank"
              rel="noopener"
              class="transition-colors duration-150 ease-out text-[#009DED]"
            >
              <!-- <i class="fab fa-twitter fa-2x"></i> -->
              <img src="@/assets/img/ico-twitter.png" alt="icono twitter" class="w-8 lg:w-20" />
            </a>
            <a
              href="https://www.twitch.tv/ao20oficial"
              target="_blank"
              rel="noopener"
              class="transition-colors duration-150 ease-out text-[#009DED]"
            >
              <!-- <i class="fab fa-twitter fa-2x"></i> -->
              <img src="@/assets/img/ico-twitch.png" alt="icono twitch" class="w-8 lg:w-20" />
            </a>
            <a
              href="https://steamcommunity.com/app/1956740/discussions/"
              target="_blank"
              rel="noopener"
              class="transition-colors duration-150 ease-out text-[#009DED]"
            >
              <!-- <i class="fab fa-twitter fa-2x"></i> -->
              <img src="@/assets/img/ico-forum.png" alt="icono foro" class="w-8 lg:w-20" />
            </a>
            <!-- <a href="#" target="_blank" class="transition-colors duration-150 ease-out hover:text-primary">
              <i class="fab fa-instagram"></i>
            </a> -->
          </div>
        </div>
      </div>

    </section>

    <div class="container-flex h-3 bg-divider-texture bg-repeat-x bg-center"></div>

    <section id="juga-gratis" class="container-flex py-12 bg-image-texture">

      <h2 class="section-title text-center mb-4">¡Jugá Gratis!</h2>

      <div class="max-w-screen-lg mx-auto grid grid-cols-1">
        <div class="flex flex-col items-center mt-12 lg:mt-12 xl:mt-16">
          <div class="relative mb-4 z-10">
            <!--
            No borrar matomo_download por que se usa para contar descarga en analytics.
            https://matomo.org/faq/new-to-piwik/faq_47/
            -->
            <a id="download-btn" href="https://store.steampowered.com/app/1956740/Argentum_20/" class="btn btn-cta matomo_download">Descargar</a>
          </div>

          <!-- <img src="@/assets/img/wings.png" alt class="absolute top-0 inset-x-auto" /> -->
          <p class="text-sm text-white mb-6">Sólo disponible para Windows</p>

          <label class="px-6 text-center">
            <span>
              Al descargar el juego en Steam declaro que leí y acepto
              <NuxtLink to="/reglamento" class="text-primary hover:underline"> el reglamento de juego </NuxtLink>
            </span>
          </label>
        </div>
        <!-- <RegisterForm /> -->
      </div>
    </section>

    <div class="container-flex h-3 bg-divider-texture bg-repeat-x bg-center"></div>
    <br>
    <br>

    <section id="newsletter" class="container max-w-screen-lg mx-auto">
      <h3 class="section-title mb-6 text-center">Newsletter</h3>
      <form
        action="https://tinyletter.com/ao20"
        method="post"
        target="popupwindow"
        onsubmit="window.open('https://tinyletter.com/ao20', 'popupwindow', 'scrollbars=yes,width=800,height=600');return true"
      >
        <p class="text-center w-full text-xl mb-4">
          <label for="tlemail">¡Recibí las novedades en tu casilla de email!</label>
        </p>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
            <div class="text-center md:text-right"><input type="text" class="w-52 h-14" name="email" id="tlemail" placeholder="Escribí tu email..." /></div>
            <div class="text-center md:text-left">
                <input type="hidden" value="1" name="embed" />
                <input type="submit" class="btn btn-silver self-start text-base" value="Subscribirse" />
            </div>
        </div>
      </form>
    </section>

    <br>
    <br>
    <div class="container-flex h-3 bg-divider-texture bg-repeat-x bg-center"></div>
    <br>
    <br>

    <section
      id="info"
      class="
        max-w-screen-xl
        mx-auto
        container
        grid
        items-center
        grid-cols-1
        md:grid-cols-6
        lg:grid-cols-12
        gap-x-12
        mb-12
        lg:mb-0
      "
    >
      <div class="flex flex-col gap-y-6 col-span-1 order-2 lg:order-1 md:col-span-4 lg:col-span-8">
        <h2 class="text-4xl text-gr gr-gold text-center lg:text-left">El primer MMORPG 100% argentino</h2>
        <p class="text-xl">
          Argentum es un juego online multijugador, donde podés tomar el rol de un guerrero, mago, paladín y muchas
          otras clases, y explorar las tierras míticas de Argentum.
        </p>
        <p class="text-xl">
          Nació en 1999 como un juego
          <span class="text-primary font-bold">totalmente desarrollado en Argentina</span> para luego ser liberado a la
          comunidad de manera gratuita. El código es accesible a todos, permitiendo así su evolución y continuidad en el
          tiempo.
        </p>
        <p class="text-xl">
          Ver codigo fuente en <a href="https://github.com/ao-org/">GitHub</a>
        </p>
      </div>

      <figure class="col-span-1 md:col-span-2 lg:col-span-4 order-1 lg:order-2">
        <img src="@/assets/img/catapulta.png" alt="Catapulta argentum 20" class="w-full" />
      </figure>
    </section>

    <MessageBox v-if="validatedMail" status="OK" :isFloating="true">
      <p class="text-lg -mt-2">Se ha validado el mail correctamente.</p>
    </MessageBox>
  </main>
</template>

<script>
import $ from "jquery";

export default {
  async asyncData({ $prismic }) {
    const homePage = await $prismic.api.getSingle("inicio");

    return {
      homePage,
    };
  },
  data() {
    return {
      validatedMail: false,
    };
  },
  mounted() {
    window.$ = window.jQuery = $;
    require("@fancyapps/fancybox");

    $("[data-fancybox='gallery']").fancybox({
      backFocus: false,
    });

    if (this.$route.query.validada == 1) {
      this.validatedMail = true;

      setTimeout(() => {
        this.validatedMail = false;
      }, 6000);
    }
  },
  methods: {
    link(prismicObject) {
      return this.$prismic.asLink(prismicObject);
    },
  },
  head() {
    return {
      title: "AO20 - Web Oficial",
    };
  },
};
</script>

<style scoped>
h1,
h2,
h3,
h4,
h5,
h6 {
  @apply tracking-wider uppercase;
}

#download-btn {
  transition: all 150ms ease-out;
  box-shadow: 0 0 20px rgba(199, 131, 0, 0.4);
}

#download-btn::before {
  @apply absolute top-0;
  content: url("/assets/img/wings_mobile.png");
  left: 50%;
  transform: translateY(-50px) translateX(-50%);
  z-index: -1;
}

#download-btn:hover {
  box-shadow: 0 0 40px rgba(199, 131, 0, 0.7), inset 0 0 35px -10px rgba(0, 0, 0, 0.75);
}

.grecaptcha-badge {
  z-index: 999;
}

@screen md {
  #download-btn::before {
    @apply w-auto;
    content: url("/assets/img/wings.png");
    transform: translateY(-99px) translateX(-50%);
  }
}

/* #download-btn:active {
  box-shadow: inset 0 0;
} */
</style>
