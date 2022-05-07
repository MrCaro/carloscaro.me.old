<template>
  <section class="bg-gray-light py-44">
    <div class="container flex h-full px-16 justify-between">
      <p class="font-roboto text-12 font-400 text-gray-default">
        &copy; Carlos 'Charlie' Caro | Front-End Developer
      </p>
      <div class="flex gap-x-16 items-center">
        <a href="https://github.com/MrCaro" target="_blank">
          <img
            :src="`${publicPath}icons/github.svg`"
            :srcset="`${publicPath}icons/github.svg`"
            alt="Check out my github profile"
          />
        </a>
        <a href="https://linkedin.com/in/carlos-caro94/" target="_blank">
          <img
            :src="`${publicPath}icons/linkedin.svg`"
            :srcset="`${publicPath}icons/linkedin.svg`"
            alt="Check out my linkedin profile"
          />
        </a>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "Footer",
  data() {
    return {
      publicPath: process.env.BASE_URL,
    };
  },
};
</script>
