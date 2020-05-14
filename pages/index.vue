<template>
 <div class="container">
   <h1>Hello World</h1>
 </div>
</template>

<script>
export default {
  head() {
    return {
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },
};
</script>

<style lang="scss">
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}

</style>
