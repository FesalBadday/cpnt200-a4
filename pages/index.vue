<template>
  <div>
    <Navigation />
    <Header :pageInfo="siteInfo" />
    <Home :pageInfo="siteInfo" />
    <Footer :pageInfo="siteInfo" />
  </div>
</template>
<script>
export default {
  data() {
    return {
      siteInfo: {
        pageName: "Carizzle",
        author: "Fesal",
        image: "images/bg-img.jpg",
      },
    };
  },
};
</script>
