<template>
  <div class="bg-white rounded-md shadow-xl">
    <h3 class="text-xl font-semibold text-center pt-1 pb-2">{{ title }}</h3>
    <div class="grid grid-cols-2 gap-x-1">
      <div class="w-full col-span-2 overflow-hidden">
        <img
          :src="foto"
          :alt="title"
          class="object-cover hover:scale-125 ease-in-out duration-300"
        />
      </div>

      <Knop
        text="View Project"
        class="bg-emerald-500 my-1"
        :link="linkProject"
      ></Knop>

      <Knop
        text="Github Code"
        class="bg-slate-500 my-1"
        :link="linkCode"
      ></Knop>

    </div>
  </div>
</template>

<script>
import Knop from "./Knop.vue";
export default {
  props: ["title", "linkCode", "linkProject", "foto"],
  components: { Knop },
};
</script>
