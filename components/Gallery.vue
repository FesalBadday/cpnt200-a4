<template>
  <div>
    <figure>
      <h3>{{ info.title }}</h3>
      <nuxt-img :src="info.image" sizes="sm:300px md:400px lg:500px" />
      <figcaption>{{ info.description }}</figcaption>
      <p>{{ info.credit }}</p>
    </figure>
  </div>
</template>
<script>
export default {
  props: ["pageInfo", "info"],
};
</script>