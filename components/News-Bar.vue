<template>
  <div class="container">
    <ul
      v-if="newsItems && newsItems.length"
      class="max-w-screen-md mx-auto bg-gray-900 border-2 border-gr border-gr-primary p-4 md:p-6"
    >
      <a v-for="currentNew in newsItems"
        :key="currentNew.gid"
        :id="currentNew.gid"
        :href="currentNew.url"
        target="_blank"
        class="group flex flex-col p-3 md:p-6 border-b last:border-b-0 border-gray-700 hover:bg-white hover:bg-opacity-10 transition-colors duration-200 ease-out"
      >
        <h1 class="text-2xl text-primary group-hover:text-white transition-colors duration-200 ease-out">
          {{ currentNew.title }}
        </h1>
        <span>
          {{ currentNew.feedlabel }}
        </span>
        <time
          :datetime="currentNew.date"
          :title="$dayjs(currentNew.date).format('DD [de] MMMM [de] YYYY [a las] HH:mm')"
        >
          {{ $dayjs(currentNew.date).format('DD [de] MMMM [de] YYYY [a las] HH:mm') }}
        </time>
      </a>
    </ul>

    <section v-else class="text-center mt-24">
      <p class="text-2xl">Aún no hay noticias.</p>
    </section>
  </div>
</template>

<script>

export default {
  data() {
    return {
      newsItems: []
    }
  },
  async fetch() {
    try {
      const news = await this.$axios.$get('https://api.steampowered.com/ISteamNews/GetNewsForApp/v0002/?appid=1956740&count=10&maxlength=300&format=json')
      let newsItems = news.appnews.newsitems

      newsItems.forEach(element => {
        element.date = element.date * 1000;
      });

      this.newsItems = newsItems
    } catch (error) {
      console.error(error)
    }

  },
  head() {
    return {
      title: "Noticias",
    };
  },
};
</script>

<style>
.news_body {
  @apply text-gray-200;
}

.news_body h1,
.news_body h2,
.news_body h3,
.news_body h4,
.news_body h5,
.news_body h6 {
  @apply mb-4 mt-6 md:mb-8 md:mt-12;
}

.news_body h1,
.news_body h2,
.news_body h3 {
  @apply border-b border-gray-800;
}

.news_body h4,
.news_body h5,
.news_body h6 {
  @apply text-xl mb-2 mt-6 md:mb-4 md:mt-8;
}

.news_body h1 {
  @apply text-3xl md:text-4xl pb-4 border-b border-gray-800;
}

.news_body h2 {
  @apply text-2xl md:text-3xl pb-3 border-b border-gray-800;
}

.news_body h3 {
  @apply text-xl md:text-2xl pb-3 border-b border-gray-800;
}

.news_body p {
  @apply my-2 md:my-3;
}

.news_body a {
  @apply text-primary underline;
}

.news ul {
  list-style-type: disc;
}

.news ol {
  list-style-type: decimal;
}

.news_body > ul,
.news_body > ol {
  @apply my-6;
}

.news ul,
.news ol {
  @apply pl-4;
}

.news ul > li,
.news ol > li {
  @apply pl-1;
}

.news ul > li::marker,
.news ol > li::marker {
  @apply text-gray-500;
}
</style>
