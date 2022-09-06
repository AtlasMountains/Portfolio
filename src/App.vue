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
        foto: "./FinanceClub.png",
        title: "the personal finance club",
        tags: [
          {id:1,name:'laravel'},
          {id:2,name:'livewire'},
          {id:3,name:'tailwindcss'},
          {id:4,name:'alpineJS'},
        ]
        }
      ,
      {
        id: 2,
        linkCode: "https://github.com/AtlasMountains/pizza",
        linkProject: "https://pizza.siteskip.be/",
        foto: "./PizzaZaak.png",
        title: "pizza zaak",
        tags: [
          {id:1,name:'PHP'},
          {id:2,name:'Bootstrap'}
        ]
      },
      {
        id: 3,
        linkCode: "https://github.com/AtlasMountains/kleurplaat",
        linkProject: "https://atlasmountains.github.io/kleurplaat/",
        foto: "./kleurplaat.png",
        title: "kleurplaat",
        tags: [
          {id:1,name:'javascript'},
          {id:2,name:'JSON'},
        ]
      },
      {
        id: 4,
        linkCode: "https://github.com/AtlasMountains/oefening-SCSS",
        linkProject: "https://atlasmountains.github.io/oefening-SCSS/",
        foto: "./ArtStudio.png",
        title: "oefening css",
        tags: [
          {id:1,name:'SASS/SCSS'},
        ]
      },
      {
        id: 5,
        linkCode: "https://github.com/AtlasMountains/yahtzee",
        linkProject: "https://atlasmountains.github.io/yahtzee/",
        foto: "./Yahtzee.png",
        title: "yahtzee",
        tags: [
          {id:1,name:'javascript'},
          {id:2,name:'OOP'},
          {id:3,name:'Bootstrap'},
        ]
      },
      {
        id: 6,
        linkCode: "https://github.com/AtlasMountains/portfolio",
        linkProject: "https://atlasmountains.github.io/portfolio",
        foto: "./Portfolio.png",
        title: "Portfolio",
        tags: [
          {id:1,name:'Vue'},
          {id:2,name:'tailwindcss'},
        ]
      },
    ];
  },
};
</script>
