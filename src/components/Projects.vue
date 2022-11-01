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
  <div class="grid grid-cols-1 gap-4 mt-2 md:grid-cols-2 lg:grid-cols-3">
    <div :key="app.id" v-for="app in apps">
      <Card
        :title="app.title"
        :foto="app.foto"
        :linkCode="app.linkCode"
        :linkProject="app.linkProject"
        :tags="app.tags"
      ></Card>
    </div>
  </div>
</template>
