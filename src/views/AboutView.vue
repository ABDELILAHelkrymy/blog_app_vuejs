<template>
  <div class="about">
    <h1>{{ pageName }}</h1>
    <p>{{ pageDescription }}</p>
    <WelcomeMessage />
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  data: function () {
    return {
      pageName: "About us",
      pageDescription: "This is About page",
    };
  },
  name: "AboutView",
};
</script>
