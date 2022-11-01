<template>
  <div
    class="bg-white rounded-md shadow-xl bg-gradient-to-r from-cyan-400 to-green-400"
  >
    <h3 class="pt-1 pb-2 text-xl font-semibold text-center">{{ title }}</h3>
    <div class="w-full col-span-2 overflow-hidden">
      <img
        :src="foto"
        :alt="title"
        class="object-cover duration-300 ease-in-out hover:scale-125"
      />
    </div>

    <div class="col-span-2 p-3 bg-cyan-500">
      <ul :key="tag.id" v-for="tag in tags" class="inline-flex flex-row">
        <li class="px-1">#{{ tag.name }}</li>
      </ul>
    </div>

    <div class="grid grid-cols-2">
      <Knop
        text="View Project"
        class="rounded-bl bg-emerald-400"
        :link="linkProject"
      ></Knop>

      <Knop
        text="Github Code"
        class="text-white rounded-br bg-slate-600"
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
