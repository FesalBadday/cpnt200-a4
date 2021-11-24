<template>
  <div>
    <figure>
      <div v-html="`<h3>${info.title}</h3>`"></div>
      <nuxt-img :src="info.image" sizes="sm:300px md:400px lg:500px" />
      <figcaption v-text="info.description" />
      <p v-text="info.credit" />
    </figure>
  </div>
</template>
<script>
export default {
  props: ["pageInfo", "info"],
};
</script>