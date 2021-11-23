<template>
  <div>
    <Navigation />
    <Header :pageInfo="siteInfo" :galleries="galleries" />
    <main class="flex justify-evenly gap-x-16 gap-y-16 flex-wrap p-16 bg-gray-400">
      <Gallery :pageInfo="siteInfo" v-for="gallery in galleries" :key="gallery.id" :info="gallery" />
    </main>
    <Footer :pageInfo="siteInfo" />
  </div>
</template>
<script>
export default {
  data() {
    return {
      siteInfo: {
        pageName: "Gallery",
        author: "Fesal",
      },
      galleries: [
        {
          title: "White Ford Mustang",
          description: "White Ford Mustang At Car Wash With Water Mist.",
          credit: "Jan Kopřiva",
          image: "images/gal-car-1.jpg",
        },
        {
          title: "Dodge Challenger",
          description: "Stylish Dodge Challenger With Glowing Headlights.",
          credit: "Erik Mclean",
          image: "images/gal-car-2.jpg",
        },
        {
          title: "Classic Car",
          description: "Old Sky Blue Classic Sedan With A Nice Sky Filter.",
          credit: "neil kelly",
          image: "images/gal-car-3.jpg",
        },
        {
          title: "Mercedes Benz",
          description: "White Mercedes Benz Sedan With An Epic Cloudy Weather.",
          credit: "Javier Aguilera",
          image: "images/gal-car-4.jpg",
        },
        {
          title: "Audi R8",
          description: "Audi R8 Parked Under The Shadow Of Trees During Fall.",
          credit: "Vlad Alexandru Popa",
          image: "images/gal-car-5.jpg",
        },
        {
          title: "Audi A5 Coupé",
          description: "Front Of A Shiny Yellow Audi A5 Coupé At Car Showroom.",
          credit: "Sourav Mishra",
          image: "images/gal-car-6.jpg",
        },
      ],
    };
  },
};
</script>