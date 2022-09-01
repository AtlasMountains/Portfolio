<template>
  <div class="bg-white rounded-md shadow-xl">
    <h3 class="text-xl font-semibold text-center pt-1 pb-2">{{ title }}</h3>
    <div class="w-full col-span-2 overflow-hidden">
      <img
          :src="foto"
          :alt="title"
          class="object-cover hover:scale-125 ease-in-out duration-300"
        />
    </div>

    <div class="p-3 bg-cyan-500 col-span-2">
      <ul :key="tag.id" v-for="tag in tags" class="flex-row inline-flex">
        <li class="px-1">#{{ tag.name }}</li>
      </ul>
    </div>

    <div class="grid grid-cols-2">
      <Knop
        text="View Project"
        class="bg-emerald-500 rounded-bl"
        :link="linkProject"
      ></Knop>

      <Knop
        text="Github Code"
        class="bg-slate-500 rounded-br"
        :link="linkCode"
      ></Knop>
    </div>
  </div>
</template>

<script>
import Knop from "./Knop.vue";
export default {
  props: ["title", "linkCode", "linkProject", "foto", "tags"],
  components: { Knop },
};
</script>
