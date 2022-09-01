<script>
import Card from "./Card.vue";
export default {
  name: "Projects",
  props: {
    apps: Array,
  },
  components: { Card },
};
</script>

<template>
  <div class="mt-2 grid gap-4 grid-cols-1 md:grid-cols-2 lg:grid-cols-3">
    <div :key="app.id" v-for="app in apps">
      <Card
        :title="app.title"
        :foto="app.foto"
        :linkCode="app.linkCode"
        :linkProject="app.linkProject"
      ></Card>
    </div>
  </div>
</template>
