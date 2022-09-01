<script setup>
import Header from "./components/Header.vue";
import Projects from "./components/Projects.vue";
</script>

<template>
  <div>
    <Header></Header>
    <Projects :apps="apps"></Projects>
  </div>
</template>

<script>
export default {
  components: {
    Header,
    Projects,
  },
  data() {
    return {
      apps: [],
    };
  },
  created() {
    this.apps = [
      {
        id: 1,
        linkCode: "https://github.com/AtlasMountains/personal-finance-club",
        linkProject: "https://siteskip.be/",
        foto: "/src/assets/FinanceClub.png",
        title: "the personal finance club",
      },
      {
        id: 2,
        linkCode: "https://github.com/AtlasMountains",
        linkProject: "https://pizza.siteskip.be/",
        foto: "/src/assets/PizzaZaak.png",
        title: "pizza zaak",
      },
      {
        id: 3,
        linkCode: "https://github.com/AtlasMountains/kleurplaat",
        linkProject: "https://atlasmountains.github.io/kleurplaat/",
        foto: "/src/assets/kleurplaat.png",
        title: "kleurplaat",
      },
      {
        id: 4,
        linkCode: "https://github.com/AtlasMountains/oefening-SCSS",
        linkProject: "https://atlasmountains.github.io/oefening-SCSS/",
        foto: "/src/assets/ArtStudio.png",
        title: "oefening css",
      },
      {
        id: 5,
        linkCode: "https://github.com/AtlasMountains/yahtzee",
        linkProject: "https://atlasmountains.github.io/yahtzee/",
        foto: "/src/assets/YahtzeeSmall.png",
        title: "yahtzee",
      },
    ];
  },
};
</script>
